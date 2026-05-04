<template>
  <div
    class="relative p-6 rounded-xl border text-white transition-all duration-300"
    :class="[
      'bg-white/5 backdrop-blur-md border-white/20',
      highlight ? ' border-purple-500 shadow-xl' : ''
    ]"
  >

    <!-- BADGE -->
    <span
      v-if="badge"
      class="absolute top-4 right-4 text-xs bg-orange-500 text-white px-2 py-1 rounded-full"
    >
      {{ badge }}
    </span>

    <!-- TITLE -->
    <h3 class="text-sm text-gray-300">{{ title }}</h3>

    <!-- PRICE -->
    <div class="mt-2 mb-4">
      <span v-if="!custom" class="text-3xl font-bold text-white">
        ${{ price }}
      </span>
      <span v-if="!custom" class="text-sm text-gray-400">/month</span>

      <span v-if="custom" class="text-2xl font-semibold">
        Contact Us
      </span>
    </div>

    <div class="h-px bg-white/20 my-4"></div>

    <!-- FEATURES -->
    <ul class="space-y-3 text-sm text-gray-300">
      <li v-for="(item, i) in features" :key="i" class="flex gap-2">
        <span class="text-green-400">✔</span>
        {{ item }}
      </li>
    </ul>

    <!-- BUTTON -->
    <button
      class="mt-6 w-full py-2 rounded-lg border border-white/20 hover:bg-white/10 transition"
      :class="highlight ? 'bg-purple-600 border-none' : ''"
    >
      Get Started
    </button>

  </div>
</template>

<script setup>
defineProps({
  title: String,
  price: String,
  features: Array,
  highlight: Boolean,
  badge: String,
  custom: Boolean
})
</script>