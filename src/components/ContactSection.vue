<template>
  <section class="bg-beige text-moss py-20 px-4">
    <div class="max-w-5xl mx-auto">
      <h2 class="text-3xl md:text-4xl font-serif text-wood text-center mb-4">
        Let’s connect over something beautifully made.
      </h2>
      <p class="text-lg md:text-xl text-center mb-10">
        Whether you're curious about a workshop, interested in stocking our pieces, or simply dreaming of a trip to Kinsale — we’d love to hear from you.
        Drop us a message and we’ll get back to you with care.
      </p>

      <div class="grid md:grid-cols-2 gap-10">
        <!-- Contact Info -->
        <div>
          <ul class="space-y-4 text-base">
            <li>27 Main Street, Kinsale, County Cork, Ireland</li>
            <li>+353 (0)21 555 1234</li>
            <li>hello@willowandwild.ie</li>
          </ul>

          <!-- Social Links -->
          <div class="flex space-x-4 mt-6">
            <a href="https://instagram.com" target="_blank" rel="noopener noreferrer" aria-label="Instagram" class="fab fa-instagram"></a>
            <a href="https://pinterest.com" target="_blank" rel="noopener noreferrer" aria-label="Pinterest" class="fa-brands fa-pinterest"></a>
            <a href="https://facebook.com" target="_blank" rel="noopener noreferrer" aria-label="Facebook" class="fab fa-facebook"></a>
          </div>

          <!-- Map -->
          <div class="mt-8">
            <iframe class="w-full h-64 rounded-2xl"
              src="https://www.google.com/maps?q=27+Main+Street,+Kinsale,+Ireland&output=embed"
              allowfullscreen loading="lazy">
            </iframe>
          </div>
        </div>

        <!-- Contact Form -->
        <form class="space-y-4 pt-13">
          <div>
            <label class="block text-sm font-medium">Name</label>
            <input type="text" class="w-full border border-moss p-2 rounded-md" required />
          </div>
          <div>
            <label class="block text-sm font-medium">Email</label>
            <input type="email" class="w-full border border-moss p-2 rounded-md" required />
          </div>
          <div>
            <label class="block text-sm font-medium">Message</label>
            <textarea class="w-full border border-moss p-2 rounded-md" rows="5" required></textarea>
          </div>
          <button type="submit" class="bg-moss text-white px-6 py-3 rounded-xl font-sans hover:bg-moss/90 transition">
            Send Message
          </button>
        </form>
      </div>
    </div>
  </section>
</template>

<script setup>

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
