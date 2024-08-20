<template>
    <div class="w-4/5 h-64 relative mx-auto mb-12">
        <div id="map" class="w-full h-full"></div>
        <button class="absolute bottom-4 right-4 bg-blue-500 text-white py-2 px-4 rounded" @click="openInGPS">
            Ir a la ubicación
        </button>
    </div>
  </template>  
  
  <script>
  import { Loader } from '@googlemaps/js-api-loader';
  
  export default {
    data() {
      return {
        map: null,
        location: { lat: 20.680707, lng: -103.368717 }, 
      };
    },
    mounted() {
      this.initMap();
    },
    methods: {
      initMap() {
        const loader = new Loader({
          apiKey: 'AIzaSyAVnrb5NFtR8trbZR2klnqOGoHZbHxPbyY',
          version: 'weekly',
        });
  
        loader.load().then(() => {
          this.map = new google.maps.Map(document.getElementById('map'), {
            center: this.location,
            zoom: 15,
          });
  
          new google.maps.Marker({
            position: this.location,
            map: this.map,
          });
        });
      },
      openInGPS() {
        const url = `https://www.google.com/maps/dir/?api=1&destination=${this.location.lat},${this.location.lng}`;
        window.open(url, '_blank');
      },
    },
  };
  </script>
  
  <style scoped>
  #map {
    width: 100%;
    height: 100%;
  }
  </style>
  