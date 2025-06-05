<template>
  <section
    id="hero"
    class="relative h-screen flex items-center justify-center text-center text-pure overflow-hidden">
    <img src="/src/assets/natura.jpg"
      alt="Siobhan and Aisling" class="absolute inset-0 w-full h-full object-cover filter brightness-75"
      aria-hidden="true"
    />
    <div
      class="relative bg-beige/80 backdrop-blur-xl p-8 md:p-16 max-w-2xl rounded-xl shadow-lg mx-auto text-center"
      data-aos="fade-up"
    >
      <h1 class="text-4xl md:text-5xl font-serif text-moss mb-4">
        Crafting Nature’s Essence
      </h1>
      <p class="text-lg md:text-xl font-sans text-wood mb-6">
        Discover unique artisanal products and experiences inspired by the wild beauty of the Irish
        south.
      </p>
      <div class="flex flex-col md:flex-row gap-4 justify-center">
        <a
          href="#contact"
          class="bg-moss text-white px-6 py-3 rounded-xl font-sans hover:bg-moss/90 transition"
        >
          Shop Handmade
        </a>
      </div>
    </div>
  </section>
</template>


<script setup>
import bgImage from '@/assets/natura.jpg'

</script>

<style scoped>
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
