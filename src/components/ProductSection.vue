<template>
  <section class="bg-beige text-moss py-20 px-4">
    <div class="max-w-5xl mx-auto text-center">
      <h2 class="text-3xl md:text-4xl font-serif text-wood mb-6">Products</h2>
      <p class="text-lg md:text-xl font-sans mb-12">
        From soothing soy candles to hand-thrown pottery, our collections reflect the rhythm of nature and the soul of Irish artistry.
      </p>

      <div class="grid gap-8 md:grid-cols-2 text-left">
        <div v-for="(item, index) in categories" :key="index" class="bg-white shadow-md rounded-2xl p-6">
          <h3 class="text-xl font-semibold text-wood mb-2">{{ item.title }}</h3>
          <p class="text-moss font-sans">{{ item.description }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const categories = [
  {
    title: 'Candles with soul',
    description: 'Hand-poured with locally inspired scents'
  },
  {
    title: 'Natural soaps',
    description: 'Kind to your skin and the planet'
  },
  {
    title: 'Herbal teas',
    description: 'Wild, warming, and wellness-focused'
  },
  {
    title: 'Art & Ceramics',
    description: 'Crafted by local makers'
  },
  {
    title: 'Textiles & Wool',
    description: 'Soft, traditional, and timeless'
  },
  {
    title: 'Preserves & Honey',
    description: 'Small-batch goodness from nearby farms'
  },
  {
    title: 'Art Prints & Postcards',
    description: 'Snapshots of the Irish coast'
  }
]
</script>
