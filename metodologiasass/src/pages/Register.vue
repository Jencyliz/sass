<template>
    <div class="register">
      <form @submit.prevent="handleRegister">
        <input type="text" placeholder="Nombre de usuario" v-model="username" />
        <input type="password" placeholder="Contraseña" v-model="password" />
        <button type="submit">Registrar</button>
      </form>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        username: '',
        password: '',
      };
    },
    methods: {
      handleRegister() {
        this.$router.push('/login');
      },
    },
  };
  </script>
  