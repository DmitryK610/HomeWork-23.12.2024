<template>
<header>
    <nav>
      <router-link to="/"><span>Главная</span></router-link>
      <router-link to="/about"><span>О нас</span></router-link>
      <router-link to="/contact"><span>Связаться с нами</span></router-link>
    </nav>
  </header>
  </template>
  <script lang="ts">
  import { defineComponent, ref } from 'vue'
  export default defineComponent({
    name: 'Header',
  });
  </script>
  
  <style scoped>
 
  nav {
    justify-content: center;
    box-shadow: 0 0 2px 2px rgb(230, 252, 230) inset;
    background-image: url(/image/forest.jpg);
    display: flex;
    gap: 20px;
    height: 30px;
    align-items: center;
  }
span
{
  color: white;
  font-size: large;

}
@media only screen and (max-width: 560px) 
{
  nav
  {
height: 150px;
flex-direction: column;
  }
}
  </style>