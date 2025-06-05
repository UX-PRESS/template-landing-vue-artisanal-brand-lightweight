<template>
  <section class="bg-beige text-moss py-20 px-4">
    <div class="max-w-5xl mx-auto">
      <h2 class="text-3xl md:text-4xl font-serif text-wood text-center mb-4">
        We’d love to hear from you.
      </h2>
      <p class="text-lg md:text-xl text-center mb-10">
        Have a question, want to collaborate, or planning a visit to Kinsale? Reach out — we’re always happy to connect.
      </p>

      <div class="grid md:grid-cols-2 gap-10">
        <!-- Contact Info -->
        <div>
          <ul class="space-y-4 text-base">
            <li>📍 27 Main Street, Kinsale, County Cork, Ireland</li>
            <li>☎️ +353 (0)21 555 1234</li>
            <li>✉️ hello@willowandwild.ie</li>
          </ul>

          <!-- Social Links -->
          <div class="flex space-x-4 mt-6">
            <a href="https://instagram.com" target="_blank" aria-label="Instagram" class="hover:text-wood">📷</a>
            <a href="https://pinterest.com" target="_blank" aria-label="Pinterest" class="hover:text-wood">📌</a>
            <a href="https://facebook.com" target="_blank" aria-label="Facebook" class="hover:text-wood">📘</a>
          </div>

          <!-- Map -->
          <div class="mt-8">
            <iframe
              class="w-full h-64 rounded-2xl"
              src="https://www.google.com/maps?q=27+Main+Street,+Kinsale,+Ireland&output=embed"
              allowfullscreen
              loading="lazy">
            </iframe>
          </div>
        </div>

        <!-- Contact Form -->
        <form class="space-y-4">
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
          <button type="submit" class="bg-wood text-beige px-6 py-2 rounded-md hover:bg-moss transition">
            Send Message
          </button>
        </form>
      </div>
    </div>
  </section>
</template>

<script setup>

</script>
