<script setup>
import Navbar from './Components/Navbar.vue';
import Main from './Components/Main.vue'
import Contact from './Components/Contact.vue';
import Hero from './Components/hero/Hero.vue'
import Especialities from './Components/specialities/Especialities.vue';
import Maps from './Components/maps/Maps.vue';
import Carousel from './components/carrusel/Carousel.vue';
import Services from './components/services/Services.vue';
import Footer from './components/footer/footer.vue';
</script>

<template>
<Navbar></Navbar>
<Hero></Hero>
<Main></Main>
<Especialities></Especialities>
  <Contact></Contact>
    <Maps></Maps>



    <Carousel />
    <Services />
    <Footer />

</template>

<style scoped>

</style>
