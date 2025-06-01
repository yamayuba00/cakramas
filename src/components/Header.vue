<!-- Navbar.vue -->
<template>
  <nav class="bg-white shadow-lg fixed w-full z-50">
    <div class="max-w-7xl mx-auto px-4">
      <div class="flex justify-between items-center py-4">
        <div class="flex items-center space-x-4">
          <div class="flex items-center">
            <div
              class="w-10 h-10 rounded-full bg-gradient-to-r from-yellow-500 to-orange-500 flex items-center justify-center"
            >
            <i class="fa fa-bars"></i>

              <!-- <i class=" fa fa-solid fa-circle-notch text-white"></i> -->
            </div>
            <span class="ml-2 font-bold text-xl text-gray-800">GCI</span>
          </div>
        </div>
        <div class="hidden md:flex items-center space-x-8">
          <a href="#home" class="text-gray-800 hover:text-orange-500 transition"
            >Home</a
          >
          <a
            href="#about"
            class="text-gray-800 hover:text-orange-500 transition"
            >About</a
          >
          <a
            href="#values"
            class="text-gray-800 hover:text-orange-500 transition"
            >Values</a
          >
          <a
            href="#mission"
            class="text-gray-800 hover:text-orange-500 transition"
            >Mission</a
          >
          <a
            href="#solutions"
            class="text-gray-800 hover:text-orange-500 transition"
            >Solutions</a
          >
          <a
            href="#contact"
            class="text-gray-800 hover:text-orange-500 transition"
            >Contact</a
          >
        </div>
        <div class="md:hidden">
          <button @click="toggleMenu" class="text-gray-800 focus:outline-none">
            <i class="fa-solid fa-bars text-xl"></i>
            <!-- <font-awesome-icon :icon="['fas', 'bars']" /> -->
          </button>
        </div>
      </div>
    </div>

    <!-- Mobile menu -->
    <div v-show="isMobileMenuOpen" class="md:hidden bg-white pb-4 px-4">
      <a
        href="#home"
        class="block py-2 text-gray-800 hover:text-orange-500 transition"
        >Home</a
      >
      <a
        href="#about"
        class="block py-2 text-gray-800 hover:text-orange-500 transition"
        >About</a
      >
      <a
        href="#values"
        class="block py-2 text-gray-800 hover:text-orange-500 transition"
        >Values</a
      >
      <a
        href="#mission"
        class="block py-2 text-gray-800 hover:text-orange-500 transition"
        >Mission</a
      >
      <a
        href="#solutions"
        class="block py-2 text-gray-800 hover:text-orange-500 transition"
        >Solutions</a
      >
      <a
        href="#contact"
        class="block py-2 text-gray-800 hover:text-orange-500 transition"
        >Contact</a
      >
    </div>
  </nav>
</template>

<script setup>
import { ref } from "vue";

const isMobileMenuOpen = ref(false);

function toggleMenu() {
  isMobileMenuOpen.value = !isMobileMenuOpen.value;
}
</script>
