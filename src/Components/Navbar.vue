<template>
    <Disclosure as="nav" class="bg-white shadow" v-slot="{ open }">
      <div class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8">
        <div class="relative flex h-16 justify-between">
          <div class="absolute inset-y-0 left-0 flex items-center sm:hidden">
            <!-- Mobile menu button -->
            <DisclosureButton class="relative inline-flex items-center justify-center rounded-md p-2 text-gray-400 hover:bg-gray-100 hover:text-gray-500 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-indigo-500">
              <span class="absolute -inset-0.5" />
              <span class="sr-only">Open main menu</span>
              <Bars3Icon v-if="!open" class="block h-6 w-6" aria-hidden="true" />
              <XMarkIcon v-else class="block h-6 w-6" aria-hidden="true" />
            </DisclosureButton>
          </div>
          <div class="flex flex-1 items-center justify-center sm:items-stretch sm:justify-between">
            <div class="flex flex-shrink-0 items-center">
              <img class="h-14 w-auto" src="../assets/logo.png" alt="Your Company" />
            </div>
            <div class="hidden sm:ml-6 sm:flex sm:space-x-8 sm:items-center">
              <!-- Current: "border-indigo-500 text-gray-900", Default: "border-transparent text-gray-500 hover:border-gray-300 hover:text-gray-700" -->
              <button type="button" class="rounded-lg  bg-blue-500 px-4 py-1 text-sm font-normal text-white shadow-sm hover:bg-blue-600 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600 items-center">Inicio</button>
              <a href="#" class="inline-flex items-center border-b-2 border-transparent px-1 pt-1 text-sm font-normal text-gray-500 hover:border-gray-300 hover:text-gray-700">Contacto</a>
              <a href="#" class="inline-flex items-center border-b-2 border-transparent px-1 pt-1 text-sm font-normal text-gray-500 hover:border-gray-300 hover:text-gray-700">Especialidad</a>
              <a href="#" class="inline-flex items-center border-b-2 border-transparent px-1 pt-1 text-sm font-normal text-gray-500 hover:border-gray-300 hover:text-gray-700">Historia</a>
              <a href="#" class="inline-flex items-center border-b-2 border-transparent px-1 pt-1 text-sm font-normal text-gray-500 hover:border-gray-300 hover:text-gray-700">Servicios</a>

            </div>
          </div>
          <div class="absolute inset-y-0 right-0 flex items-center pr-2 sm:static sm:inset-auto sm:ml-6 sm:pr-0">

  
            <!-- Profile dropdown -->

          </div>
        </div>
      </div>
  
      <DisclosurePanel class="sm:hidden">
        <div class="space-y-1 pb-4 pt-2">
          <!-- Current: "bg-indigo-50 border-indigo-500 text-indigo-700", Default: "border-transparent text-gray-500 hover:bg-gray-50 hover:border-gray-300 hover:text-gray-700" -->
          <DisclosureButton as="a" href="#" class="block border-l-4 border-indigo-500 bg-indigo-50 py-2 pl-3 pr-4 text-base font-medium text-indigo-700">Dashboard</DisclosureButton>
          <DisclosureButton as="a" href="#" class="block border-l-4 border-transparent py-2 pl-3 pr-4 text-base font-medium text-gray-500 hover:border-gray-300 hover:bg-gray-50 hover:text-gray-700">Contacto</DisclosureButton>
          <DisclosureButton as="a" href="#" class="block border-l-4 border-transparent py-2 pl-3 pr-4 text-base font-medium text-gray-500 hover:border-gray-300 hover:bg-gray-50 hover:text-gray-700">Especialidades</DisclosureButton>
          <DisclosureButton as="a" href="#" class="block border-l-4 border-transparent py-2 pl-3 pr-4 text-base font-medium text-gray-500 hover:border-gray-300 hover:bg-gray-50 hover:text-gray-700">Historia</DisclosureButton>
          <DisclosureButton as="a" href="#" class="block border-l-4 border-transparent py-2 pl-3 pr-4 text-base font-medium text-gray-500 hover:border-gray-300 hover:bg-gray-50 hover:text-gray-700">Servicios</DisclosureButton>

        </div>
      </DisclosurePanel>
    </Disclosure>
  </template>
  
  <script setup>
  import { Disclosure, DisclosureButton, DisclosurePanel, Menu, MenuButton, MenuItem, MenuItems } from '@headlessui/vue'
  import { Bars3Icon, BellIcon, XMarkIcon } from '@heroicons/vue/24/outline'

  
  </script>