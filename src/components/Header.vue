<!--src/components/Header.vue ---->  
<template>
  <header class="bg-beige shadow-md fixed w-full z-50" data-aos="fade-down">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex justify-between items-center h-16">
      <!-- Logo -->
      <div class="flex items-center space-x-2">
        <img :src="logo" alt="Willow & Wild Logo" class="h-8 w-8" />
        <span class="text-wood text-xl font-serif">Willow & Wild</span>
      </div>

      <!-- Desktop Navigation -->
      <nav class="hidden md:flex space-x-8 text-moss font-sans text-sm">
        <a href="#hero" class="hover:text-wood transition">Home</a>
        <a href="#about" class="hover:text-wood transition">About</a>
        <a href="#products" class="hover:text-wood transition">Products</a>
        <a href="#contact" class="hover:text-wood transition">Contact</a>
      </nav>

      <!-- Mobile Menu Button -->
      <div class="md:hidden">
       <button @click="isOpen = !isOpen" class="text-moss focus:outline-none">
         <span v-if="!isOpen">☰</span> <!-- menu opened -->
         <span v-else>✕</span>          <!-- menu opened -->
      </button>
      </div>
    </div>

    <!-- Mobile Dropdown -->
    <div
      v-if="isOpen"
      class="md:hidden bg-beige px-4 pb-4 flex flex-col space-y-2 text-moss font-sans text-sm"
    >
      <a href="#hero" class="hover:text-wood transition">Home</a>
      <a href="#about" class="hover:text-wood transition">About</a>
      <a href="#products" class="hover:text-wood transition">Products</a>
      <a href="#contact" class="hover:text-wood transition">Contact</a>
    </div>

</header>
</template>

<script setup>
import logo from '@/assets/logo.png'
import { ref, onMounted } from 'vue'
import AOS from 'aos'
import 'aos/dist/aos.css'

const isOpen = ref(false)

onMounted(() => {
  AOS.init({
    duration: 800,
    easing: 'ease-in-out',
    once: true,
  })
})
</script>

<style scoped>
header {
  transition: all 0.3s ease;
}
</style>
