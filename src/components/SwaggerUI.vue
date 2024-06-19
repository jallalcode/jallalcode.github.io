<!-- src/components/SwaggerUI.vue -->
<template>
    <div id="swagger-ui"></div>
  </template>
  
  <script>
  import SwaggerUI from 'swagger-ui-dist/swagger-ui-es-bundle';
  import 'swagger-ui-dist/swagger-ui.css';
  
  export default {
    name: 'SwaggerUI',
    mounted() {
      SwaggerUI({
        url: 'https://toolboxapi.online/v3/api-docs',
        dom_id: '#swagger-ui',
      });
    },
  };
  </script>
  
  <style scoped>
  #swagger-ui {
    margin: 20px;
  }
  </style>
  