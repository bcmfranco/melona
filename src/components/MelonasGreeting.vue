<template>
    <div class="card">
      <button class="mdc-button" type="button" @click="generateGreeting">🍈</button>
      <p v-show="showGreeting" class="mdc-typography--body1">{{ greeting }}</p>
    </div>
  </template>
  
  <script setup>
  import { ref } from 'vue';
  
  let greeting = ref('');
  let showGreeting = ref(false);
  
  const generateGreeting = () => {
    greeting.value = 'hola melona';
    showGreeting.value = true;
  
    setTimeout(() => {
      showGreeting.value = false;
    }, 2000);
  };
  </script>
  
  <style scoped>
  .card {
    display: grid;
    flex-direction: 70% 30%;
    text-align: center;
    padding: 20px;
  }
  
  .mdc-button {
    background-color: var(--lemon);
    color: #fff;
    border: none;
    border-radius: 4px;
    padding: 10px 20px;
    font-size: 120px;
    cursor: pointer;
    transition: background-color 0.3s;
  }
  
  .mdc-button:hover {
    background-color: #a7a7a7;
  }
  
  .mdc-typography--body1 {
    font-size: 40px;
    color: rgb(33, 33, 33);
    margin-top: 10px;
  }
  </style>
  