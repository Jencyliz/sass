<template>
    <div class="post-detail">
      <h1>{{ post.title }}</h1>
      <p>{{ post.content }}</p>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        post: {},
      };
    },
    mounted() {
      const postId = this.$route.params.id;
      // Simula la obtención de datos del post según el ID
      this.post = {
        id: postId,
        title: `Título del Post ${postId}`,
        content: `Contenido del post con ID ${postId}`,
      };
    },
  };
  </script>
  