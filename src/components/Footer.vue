<template>
    <footer>
      <p>Время работы: 10:00 - 18:00</p>
      <p>Адрес: Киров, Московская, 1</p>
    </footer>
  </template>
  
  <script lang="ts">
   import { defineComponent, ref } from 'vue'
 export default defineComponent({
    name: 'Footer',
  });
  </script>
  
  <style scoped>
  footer {
    font-size: large;
color: white;
   
 margin-top: 18px;
 backdrop-filter: blur(5px);
 box-shadow: 0 0 2px 2px rgb(250, 241, 199) inset;
   background-image: url(/image/leopard.jpg);
   background-size: 50%;
    text-align: center;
  }
  </style>