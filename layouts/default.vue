import { ref } from "#imports";

<script setup lang="ts">
const isOpen=true
</script>
<template>
  <nav class="bg-white shadow">
    <div class="container mx-auto px-6 py-3 flex justify-between items-center">
      <a href="#" class="text-xl font-semibold text-gray-700">Brand</a>
      <div class="flex-1 ml-10">
        <div class="relative max-w-sm">
          <input type="text"
            class="w-full bg-gray-100 rounded border border-gray-300 focus:border-blue-500 focus:bg-white focus:ring-0 text-base outline-none text-gray-700 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out"
            placeholder="Search">
          <div class="absolute inset-y-0 right-0 pr-3 flex items-center pointer-events-none">
            <!-- Search icon -->
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
              stroke="currentColor" class="w-5 h-5">
              <path stroke-linecap="round" stroke-linejoin="round"
                d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z" />
            </svg>

          </div>
        </div>
      </div>
      <div class="flex items-center space-x-1">
        <a href="#" class="py-2 px-3 text-gray-700 hover:text-gray-900 hidden md:block">Home</a>
        <a href="#" class="py-2 px-3 text-gray-700 hover:text-gray-900 hidden md:block">Careers</a>
        <a href="#" class="py-2 px-3 text-gray-700 hover:text-gray-900 hidden md:block">Blog</a>
        <a href="#" class="py-2 px-3 text-gray-700 hover:text-gray-900 hidden md:block">Contact Us</a>
        <a href="#"
          class="py-2 px-3 bg-blue-500 text-white rounded hover:bg-blue-600 transition duration-300 hidden md:block">Get
          Started</a>
        <button class="text-gray-700 hover:text-gray-900 md:hidden">
          <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
          </svg>
        </button>
      </div>
    </div>
    <!-- mobile menu -->
    <div :class="isOpen ? 'block' : 'hidden'" class="md:hidden">
      <a href="#" class="block py-2 px-4 text-sm hover:bg-gray-100">Home</a>
      <a href="#" class="block py-2 px-4 text-sm hover:bg-gray-100">Careers</a>
      <a href="#" class="block py-2 px-4 text-sm hover:bg-gray-100">Blog</a>
      <a href="#" class="block py-2 px-4 text-sm hover:bg-gray-100">Contact Us</a>
      <a href="#" class="block py-2 px-4 text-sm bg-blue-500 text-white rounded hover:bg-blue-600">Get Started</a>
    </div>
  </nav>
</template>