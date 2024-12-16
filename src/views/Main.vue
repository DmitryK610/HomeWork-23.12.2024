<template>
    <div class="about">
      <div class="text">
      <h1>Добро пожаловать в наш зоопарк!</h1>
      <p>Здесь вы найдете множество животных.</p>
    </div>
    </div>
  </template>
  
  <script lang="ts">
 import { defineComponent, ref } from 'vue'
 export default defineComponent({
    name: 'Main',
  });
  </script>
  <style scoped>
  .about
  {
    text-align: center;
    background-position: center center;
    background-repeat: no-repeat;
background-attachment: fixed;
   background-size: cover;
   color: white;
    background-image: url(/image/1.png);
  }
  h1
  {
    text-align: center;
  }
 .text
  {
    background-color: rgba(0, 0, 0, 0.5);
    padding: 5px;
   
  }
  </style>