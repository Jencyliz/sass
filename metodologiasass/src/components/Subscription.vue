<template>
    <div class="subscription">
      <h2>Suscríbete a nuestro blog</h2>
      <form @submit.prevent="subscribe">
        <input type="email" placeholder="Correo electrónico" v-model="email" />
        <button type="submit">Suscribirse</button>
      </form>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        email: '',
      };
    },
    methods: {
      subscribe() {
        // Lógica para suscripción
        alert(`Gracias por suscribirte con el correo: ${this.email}`);
      },
    },
  };
  </script>
  