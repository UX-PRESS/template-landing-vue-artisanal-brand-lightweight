<template>
  <section class="bg-bege text-moss py-20 px-4">
    <div class="max-w-6xl mx-auto text-center">
      <h2 class="text-3xl md:text-4xl font-serif text-wood mb-6">Products</h2>
      <p class="text-lg md:text-xl font-sans mb-12">
        From soothing soy candles to hand-thrown pottery, our collections reflect the rhythm of nature and the soul of Irish artistry.
      </p>

      <div class="grid gap-8 sm:grid-cols-2 md:grid-cols-3 text-left">
        <div
          v-for="(item, index) in visibleProducts"
          :key="index"
          class="bg-white shadow-md hover:shadow-lg transition hover:-translate-y-1 rounded-2xl p-6 cursor-pointer"
        >
          <img :src="item.image" :alt="item.title" class="w-full h-40 object-cover rounded-xl mb-4" />
          <h3 class="text-xl font-semibold text-wood mb-2">{{ item.title }}</h3>
          <p class="text-moss font-sans text-sm">{{ item.description }}</p>
        </div>
      </div>

      <div class="mt-12">
        <button class="btn btn-outline" @click="toggleView">
          {{ showAll ? 'View Less' : 'View More' }}
        </button>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref, computed } from 'vue'

const showAll = ref(false)

const categories = [
  {
    title: 'Candles with soul',
    description: 'Hand-poured with locally inspired scents',
    image: '/src/assets/candles.jpg'
  },
  {
    title: 'Natural soaps',
    description: 'Kind to your skin and the planet',
    image: '/src/assets/natural-soap.jpg'
  },
  {
    title: 'Herbal teas',
    description: 'Wild, warming, and wellness-focused',
    image: '/src/assets/herbal-teas.jpg'
  },
  {
    title: 'Art & Ceramics',
    description: 'Crafted by local makers',
    image: '/src/assets/ceramics.jpg'
  },
  {
    title: 'Textiles & Wool',
    description: 'Soft, traditional, and timeless',
    image: '/src/assets/wool.jpg'
  },
  {
    title: 'Preserves & Honey',
    description: 'Small-batch goodness from nearby farms',
    image: '/src/assets/preserves-honey.jpg'
  }
]

const visibleProducts = computed(() =>
  showAll.value ? categories : categories.slice(0, 3)
)

function toggleView() {
  showAll.value = !showAll.value
}

</script>
<style scoped>
@import url('https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css');
.text-moss {
  color: #3C5F45;
}
.bg-moss {
  background-color: #3C5F45;
}
.text-wood {
  color: #6B4F3B;
}
.bg-bege {
  background-color: #F5F1EA;
}
</style>
