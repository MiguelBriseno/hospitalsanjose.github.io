<template>
    <footer class="bg-blue-700 text-white py-8">
      <div class="container mx-auto px-4">
        <div class="flex flex-col md:flex-row justify-between items-start space-y-8 md:space-y-0">
          <!-- Logo and Social Icons -->
          <div class="w-full md:w-1/3">
            <div class="mb-4">
              <!-- Replace with your logo -->
              <!-- <img src="/path-to-your-logo.png" alt="Logo" class="h-8"> -->
            </div>
            <!-- Social Icons (optional) -->
            <!--
            <div class="flex space-x-4">
              <a aria-label="Instagram">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" class="h-6 w-6">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 8h10M7 12h8m-8 4h6m2 4h.01M4 4h16v16H4V4z" />
                </svg>
              </a>
              <a aria-label="YouTube">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" class="h-6 w-6">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 10l-5 3 5 3V10zM19 20c0-1.105-.672-2.083-1.75-2.45M5 20a4.992 4.992 0 011.75-2.45M19 4c1.105 0 2.083.672 2.45 1.75M5 4A4.992 4.992 0 017.75 2.75M12 14a4 4 0 110-8 4 4 0 010 8z" />
                </svg>
              </a>
              <a aria-label="LinkedIn">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" class="h-6 w-6">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 8a6 6 0 00-12 0v10a6 6 0 0012 0V8zM12 16v4m0 0H8m4 0h4" />
                </svg>
              </a>
            </div>
            -->
          </div>
  
          <!-- Links Section -->
          <div class="w-full md:w-2/3 flex flex-col md:flex-row space-y-8 md:space-y-0 md:space-x-16">
            <div>
              <h3 class="font-semibold mb-4">Nuestros servicios</h3>
              <ul class="space-y-2">
                <li><a href="#" class="hover:underline">Óptica</a></li>
                <li><a href="#" class="hover:underline">Farmacia</a></li>
                <li><a href="#" class="hover:underline">Exámenes de laboratorio</a></li>
                <li><a href="#" class="hover:underline">Valoración cardiológica</a></li>
                <li><a href="#" class="hover:underline">Valoración pediátrica</a></li>
                <li><a href="#" class="hover:underline">Cirugías minimamente invasivas</a></li>
                <li><a href="#" class="hover:underline">Cirugía ocular</a></li>
                <li><a href="#" class="hover:underline">Consultas</a></li>
              </ul>
            </div>
            <div>
              <h3 class="font-semibold mb-4">Nuestras especialidades</h3>
              <ul class="space-y-2">
                <li><a href="#" class="hover:underline">Oculoplástica</a></li>
                <li><a href="#" class="hover:underline">Oftalmología pediátrica</a></li>
                <li><a href="#" class="hover:underline">Retina</a></li>
                <li><a href="#" class="hover:underline">Glaucoma</a></li>
                <li><a href="#" class="hover:underline">Estrabismo</a></li>
                <li><a href="#" class="hover:underline">Cornea</a></li>
              </ul>
            </div>
            <div>
              <h3 class="font-semibold mb-4">Contacto</h3>
              <ul class="space-y-2">
                <li><a href="#" class="hover:underline">ANDRES TERAN 261 SANTA TERESITA, GUADALAJARA, JALISCO 44600</a></li>
                <li><a href="#" class="hover:underline">+52 333 825 0553</a></li>
                <li><a href="#" class="hover:underline">atencionclienteshsj1712@gmail.com</a></li>
                <li><a href="#" class="hover:underline">NO SE REALIZAN CITAS</a></li>
              </ul>
            </div>
          </div>
        </div>
  
        <!-- Footer Bottom -->
        <div class="mt-8 text-center text-sm">
          Hospital San José De Los Ojos © 2024
        </div>
      </div>
    </footer>
  </template>
  
  <script>
  export default {
    name: 'FooterComponent',
  };
  </script>
  
  <style scoped>
  /* Custom styles can go here if needed */
  </style>
  