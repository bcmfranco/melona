<template>
  <div class="card">
    <button type="button" @click="generateGreeting">Saludar</button>
    <p>{{ greeting }}</p>
  </div>
</template>

<script setup>
import { ref } from 'vue'

let greeting = ref('');
let showGreeting = ref(false);
let timerId;

const generateGreeting = () => {
  greeting.value = '¡Hola Melona!';
  showGreeting.value = true;

  clearTimeout(timerId);
  timerId = setTimeout(() => {
    showGreeting.value = false;
  }, 2000);
};
</script>

<style scoped>
    .read-the-docs {
    color: #888;
    }
    
</style>
