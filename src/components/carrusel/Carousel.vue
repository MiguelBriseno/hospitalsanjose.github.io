<template>
  <div class="relative w-full max-w-4xl mx-auto overflow-hidden pt-4 pb-4">
    <!-- Carrusel -->
    <div class="flex transition-transform duration-500 ease-in-out"
      :style="{ transform: `translateX(-${currentIndex * 100}%)` }">
      <div v-for="(slide, index) in slides" :key="index" class="flex-shrink-0 w-full flex justify-center">
        <div v-for="image in slide" :key="image" class="w-full bg-white rounded-lg shadow-lg overflow-hidden mx-2">
          <img :src="image" class="w-full h-96 object-cover" :alt="'Slide ' + (index + 1)" />
        </div>
      </div>
    </div>

    <!-- Botones de navegación -->
    <button
      class="absolute top-1/2 left-2 transform -translate-y-1/2 bg-gray-700 text-white p-2 sm:p-4 rounded-full shadow-lg hover:bg-gray-600 transition duration-300"
      @click="prevSlide">
      &#8249;
    </button>
    <button
      class="absolute top-1/2 right-2 transform -translate-y-1/2 bg-gray-700 text-white p-2 sm:p-4 rounded-full shadow-lg hover:bg-gray-600 transition duration-300"
      @click="nextSlide">
      &#8250;
    </button>

    <!-- Indicadores -->
    <div class="absolute bottom-4 left-1/2 transform -translate-x-1/2 flex space-x-2">
      <span v-for="(slide, index) in slides" :key="index" :class="[
        'h-2 w-2 rounded-full cursor-pointer',
        currentIndex === index ? 'bg-gray-800' : 'bg-gray-400'
      ]" @click="goToSlide(index)"></span>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      currentIndex: 0,
      images: [
        "https://image.lexica.art/full_webp/0bb80367-6f31-4a7d-8af2-ce6b9df042fe",
        "https://image.lexica.art/full_webp/6faf1997-be13-4773-b65f-e0c7a81ef53f",
        "https://image.lexica.art/full_webp/de80f8a7-e40f-4ef2-834e-45e1a15f072d",
        "https://image.lexica.art/full_webp/f586285e-41de-4819-9243-39fc6fe87076",
        "https://image.lexica.art/full_webp/91ef7874-d9d2-4b69-a565-b52a084dab7a",
      ],
    };
  },
  computed: {
    slides() {
      const slides = [];
      for (let i = 0; i < this.images.length; i += 2) {
        slides.push(this.images.slice(i, i + 2));
      }
      return slides;
    },
  },
  methods: {
    nextSlide() {
      this.currentIndex = (this.currentIndex + 1) % this.slides.length;
    },
    prevSlide() {
      this.currentIndex =
        (this.currentIndex - 1 + this.slides.length) % this.slides.length;
    },
    goToSlide(index) {
      this.currentIndex = index;
    },
  },
};
</script>

<style scoped>
/* Puedes agregar estilos adicionales si es necesario */
@media (max-width: 640px) {
  .flex-shrink-0 {
    width: 100%;
  }

  .w-full {
    width: 100%;
  }
}
</style>
