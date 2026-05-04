<script setup>
import { useRoute } from "vue-router";

const route = useRoute();
</script>
<template>
  <nav
    :class="[
      'w-full absolute top-0 left-0 z-50 transition-all duration-300',
      route.path === '/'
        ? 'bg-transparent text-white' // HOME
        : 'bg-white text-black shadow', // OTHER PAGES
    ]"
  >
    <div
      class="max-w-6xl mx-auto px-4 md:px-6 lg:px-8 flex items-center justify-between h-20"
    >
      <div class="flex items-center gap-2">
        <img src="/logo.png" class="h-8" />
        <span class="font-semibold text-purple-700"></span>
      </div>

      <div class="hidden md:flex gap-10">
        <NuxtLink
          to="/"
          class="text-purple-500 hover:text-purple-700 hover:font-semibold transition"
          active-class="text-purple-700 font-semibold"
        >
          Home
        </NuxtLink>

        <NuxtLink
          to="/about"
          class="text-purple-500 hover:text-purple-700 hover:font-semibold transition"
          active-class="text-purple-700 font-semibold"
        >
          About Us
        </NuxtLink>

        <NuxtLink
          to="/docs"
          class="text-purple-500 hover:text-purple-700 hover:font-semibold transition"
          active-class="text-purple-700 font-semibold"
        >
          Docs
        </NuxtLink>

        <NuxtLink
          to="/pricing"
          class="text-purple-500 hover:text-purple-700 hover:font-semibold transition"
          active-class="text-purple-700 font-semibold"
        >
          Pricing
        </NuxtLink>
      </div>

      <button class="bg-purple-700 text-white px-5 py-2 rounded-lg">
        Get Started
      </button>
    </div>
  </nav>
</template>
