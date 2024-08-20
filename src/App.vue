<script setup>
import Navbar from './Components/Navbar.vue';
import Main from './Components/Main.vue'
import Contact from './Components/Contact.vue';
</script>

<template>
<Navbar></Navbar>
  <Main></Main>
  <Contact></Contact>
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
