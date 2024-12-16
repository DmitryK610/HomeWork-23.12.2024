<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'



</script>

<template>
<div class="app">
  <Header class="header"></Header> 
  <RouterView class="router"/>
  <Footer class="footer"></Footer>
</div>
  
</template>
<style scoped>
.app
{
  display: flex;
 
  flex-direction: column;
  height: 100vh;
}
.header{
 flex: 1;
}
.router
{
flex: 20;
 
}
.footer
{
  flex: 1;
}
</style>
