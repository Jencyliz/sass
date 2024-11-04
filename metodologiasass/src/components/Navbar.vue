<template>
    <nav class="navbar">
      <div class="container">
        <router-link to="/" class="navbar-brand">Mi Blog</router-link>
        <ul class="navbar-menu">
          <li><router-link to="/register">Registro</router-link></li>
          <li><router-link to="/login">Login</router-link></li>
          <li><router-link to="/">Inicio</router-link></li>
        </ul>
      </div>
    </nav>
  </template>
  
  <script>
  export default {
    name: 'Navbar',
  };
  </script>
  
  <style scoped lang="scss">
  .navbar {
    background-color: #343a40; // Color de fondo de la barra de navegación
    padding: 15px 0; // Espaciado
    color: white; // Color del texto
  
    .container {
      max-width: 1200px; // Ancho máximo del contenedor
      margin: 0 auto; // Centrando el contenedor
      padding: 0 15px; // Espaciado lateral
      display: flex; // Usar flexbox para alinear elementos
      justify-content: space-between; // Espacio entre elementos
      align-items: center; // Centrar verticalmente
    }
  
    .navbar-brand {
      font-size: 24px; // Tamaño de la fuente de la marca
      color: white; // Color del texto de la marca
      text-decoration: none; // Sin subrayado
    }
  
    .navbar-menu {
      list-style: none; // Sin viñetas
      padding: 0; // Sin padding
      display: flex; // Usar flexbox para alinear enlaces
  
      li {
        margin-left: 20px; // Espaciado entre enlaces
      }
  
      a {
        color: white; // Color de los enlaces
        text-decoration: none; // Sin subrayado
        transition: color 0.3s; // Transición para el color
  
        &:hover {
          color: #007bff; // Color al pasar el ratón
        }
      }
    }
  }
  </style>
  