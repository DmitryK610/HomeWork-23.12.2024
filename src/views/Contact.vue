<template>
  <div class="back">
    <div class="form" >
      <h1>Связаться с нами</h1>
   
      <form  @submit.prevent="sendMessage" >
        <div class="input">
        <div >
          <label for="email">Адрес электронной почты для обратной связи</label>
          <input type="email" v-model="email" required />
        </div>
        <div>
          <label for="question">Вопрос к администрации зоопарка</label>
          <input type="text" v-model="question" required />
        </div>
      </div>
        
        <button type="submit">Отправить</button>
      </form>
    </div>
  </div>
  </template>
  
  <script lang="ts">
  import { defineComponent, ref } from 'vue'
  export default defineComponent({
    name: 'Contact',
    data() {
      return {
        question: '',
        email: '',
      
      }
    },
    methods: {
      sendMessage() {
       
        alert('Сообщение отправлено, ждите ответного письма!');
      }
    },
  });
  </script>
   <style scoped>
  h1 {
text-align: center;
color: white;
  }
  .back
  {

    background-position: center center;
    background-repeat: no-repeat;
background-attachment: fixed;
   background-size: cover;
   

  
  
    background-image: url(/image/croc.png) ;
  }
  .form
  {
   
    background-color: rgba(0, 0, 0, 0.5);
color: white;
padding: 10px;
width: 500px;
margin-right: auto;
margin-left: auto;
margin-top: 300px;
  }
  .input
  {
    display: flex;
  }
  @media only screen and (max-width: 560px) 
{

  .form
{
  width: 100%;
  padding: 0;
}

.input
{
display: flex;
flex-direction: column;
width: 100%;
}
}
   </style>
  