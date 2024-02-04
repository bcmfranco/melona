<template>
  <div>

    <h1>melona's world</h1>

    <MelonasGreeting />
  </div>
</template>

<script setup>
import MelonasGreeting from './components/MelonasGreeting.vue';



let count = 0;

</script>

<style scoped>

@font-face {
  font-family: 'Marcellus';
  src: url('assets/Marcellus-Regular.ttf') format('truetype');
}

*{
  font-family: Marcellus;
}
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
