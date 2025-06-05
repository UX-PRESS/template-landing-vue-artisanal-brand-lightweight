<!--src/components/Header.vue ---->  
<template>
  <header class="fixed top-0 left-0 w-full z-50 bg-beige/80 backdrop-blur-md shadow-sm">
    <nav class="max-w-7xl mx-auto px-4 py-3 flex justify-between items-center">
      <!-- Logo -->
      <div class="flex items-center space-x-2">
        <img :src="logo" alt="Willow & Wild Logo" class="h-8 w-8" />
        <span class="text-2xl font-serif text-moss font-bold tracking-wide">Willow & Wild</span>
      </div>

      <!-- Desktop Navigation -->
      <div class="hidden md:flex gap-6 text-wood font-sans font-medium">
        <a href="#hero" class="hover:text-wood transition">Home</a>
        <a href="#about" class="hover:text-wood transition">About</a>
        <a href="#products" class="hover:text-wood transition">Products</a>
        <a href="#contact" class="hover:text-wood transition">Contact</a>
      </div>
   
      <!-- CTA  -->
      <a href="#contact" class="bg-moss text-white px-6 py-3 rounded-xl font-sans hover:bg-moss/90 transition">
        Shop Handmade
      </a>
   
      <!-- Mobile Menu Toggle -->
      <button @click="isOpen = !isOpen" class="md:hidden text-moss">
        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path v-if="!isOpen" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"/>
          <path v-else stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"/>
        </svg>
      </button>
    </nav>

    <!-- Mobile Dropdown -->
    <div v-if="isOpen"
      class="md:hidden bg-beige px-4 pb-4 flex flex-col space-y-2 text-moss font-sans text-sm">
      <a href="#hero" class="hover:text-wood transition">Home</a>
      <a href="#about" class="hover:text-wood transition">About</a>
      <a href="#products" class="hover:text-wood transition">Products</a>
      <a href="#contact" class="hover:text-wood transition">Contact</a>
    </div>

</header>
</template>

<script setup>
import logo from '@/assets/logo1.png'
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
.text-moss {
  color: #3C5F45;
}
.bg-moss {
  background-color: #3C5F45;
}
.text-wood {
  color: #6B4F3B;
}
</style>
