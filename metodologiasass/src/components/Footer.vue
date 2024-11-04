<template>
    <footer class="footer">
      <div class="container">
        <p>&copy; {{ currentYear }} Mi Blog. Todos los derechos reservados.</p>
        <div class="social-links">
          <a href="https://facebook.com" target="_blank" rel="noopener noreferrer">Facebook</a>
          <a href="https://twitter.com" target="_blank" rel="noopener noreferrer">Twitter</a>
          <a href="https://instagram.com" target="_blank" rel="noopener noreferrer">Instagram</a>
        </div>
      </div>
    </footer>
  </template>
  
  <script>
  export default {
    data() {
      return {
        currentYear: new Date().getFullYear(),
      };
    },
  };
  </script>
  
  <style scoped lang="scss">
  .footer {
    background-color: #f8f9fa;
    padding: 20px 0;
    text-align: center;
  
    .container {
      max-width: 1200px;
      margin: 0 auto; 
      padding: 0 15px;
    }
  
    p {
      margin: 0;
    }
  
    .social-links {
      margin-top: 10px;
      a {
        margin: 0 10px;
        text-decoration: none;
        color: #007bff;
        transition: color 0.3s;
  
        &:hover {
          color: #0056b3;
        }
      }
    }
  }
  </style>
  