<template>
  <div id="world">
      <h1>melona's world</h1>
      <MelonasGreeting />
  </div>
</template>

<script setup>
import MelonasGreeting from './components/MelonasGreeting.vue';



let count = 0;

</script>

<style scoped>

:root {
  --lemon: #fcfff0;
}

@font-face {
  font-family: 'Marcellus';
  src: url('assets/Marcellus-Regular.ttf') format('truetype');
}

#app{
  background-color: red;
}

*{
  font-family: Marcellus;
}
</style>
