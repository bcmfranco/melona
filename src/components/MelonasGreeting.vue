<template>
    <div class="card">
      <button type="button" @click="generateGreeting">🍈</button>
      <p v-show="showGreeting">{{ greeting }}</p>
    </div>
  </template>
  
  <script setup>
  import { ref } from 'vue'
  
  let greeting = ref('');
  let showGreeting = ref(false);
  
  const generateGreeting = () => {
    greeting.value = '¡Hola Melona!';
    showGreeting.value = true;
  
    setTimeout(() => {
      showGreeting.value = false;
    }, 2000);
  };
  </script>
  
  <style scoped>
    .card {
      text-align: center;
    }
  
    button {
      margin-bottom: 10px;
      padding: 10px;
      font-size: 16px;
    }
  
    p {
      font-size: 18px;
      color: green;
    }
  </style>
  