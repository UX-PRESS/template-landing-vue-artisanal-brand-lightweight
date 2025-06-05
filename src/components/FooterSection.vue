<template>
  <footer class="bg-wood text-beige pt-12 pb-8 px-4">
    <div class="max-w-7xl mx-auto grid grid-cols-1 md:grid-cols-4 gap-8 text-sm">

      <!-- Logo / Sobre -->
      <div class="md:col-span-1 space-y-2">
        <h3 class="font-serif text-xl">Willow & Wild</h3>
        <p class="text-beige/80">
          Crafted by nature. Inspired by community.
        </p>
      </div>

      <!-- Navegação -->
      <div>
        <h4 class="font-semibold mb-2 uppercase tracking-wide">Explore</h4>
        <ul class="space-y-1">
          <li><a href="#about" class="hover:text-moss transition">About</a></li>
          <li><a href="#products" class="hover:text-moss transition">Products</a></li>
          <li><a href="#contact" class="hover:text-moss transition">Contact</a></li>
        </ul>
      </div>

      <!-- Contato -->
      <div>
        <h4 class="font-semibold mb-2 uppercase tracking-wide">Contact</h4>
        <ul class="space-y-1">
          <li>📍 27 Main Street, Kinsale</li>
          <li>☎️ +353 (0)21 555 1234</li>
          <li>✉️ hello@willowandwild.ie</li>
        </ul>
      </div>

      <!-- Social -->
      <div>
        <h4 class="font-semibold mb-2 uppercase tracking-wide">Follow Us</h4>
        <div class="flex space-x-4 text-xl">
          <a href="#" class="hover:text-moss transition" aria-label="Instagram">
            <i class="fab fa-instagram"></i>
          </a>
          <a href="#" class="hover:text-moss transition" aria-label="Pinterest">
            <i class="fab fa-pinterest"></i>
          </a>
          <a href="#" class="hover:text-moss transition" aria-label="Facebook">
            <i class="fab fa-facebook"></i>
          </a>
        </div>
      </div>
    </div>

    <div class="text-center text-xs text-beige/70 mt-10">
      &copy; {{ new Date().getFullYear() }} Willow & Wild. All rights reserved.
    </div>
  </footer>
</template>

<script setup>
// Nenhum JS necessário neste caso.
</script>

<style scoped>
@import url('https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css');
</style>
