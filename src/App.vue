<script setup>
import Hero from './components/hero/Hero.vue'
import Especialities from './components/specialities/Especialities.vue';
import Maps from './components/maps/Maps.vue';
</script>

<template>
  <div class="">
    <Hero/>
    <Especialities/>
    <Maps/>
  </div>
</template>

<style scoped>
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
