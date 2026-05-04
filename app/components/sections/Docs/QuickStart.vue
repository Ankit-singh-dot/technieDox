<script setup>
import { ref } from "vue";

const current = ref(0);

const steps = [
  {
    title: "Set up your workspace",
    content: [
      "Create an account or sign in with your enterprise credentials.",
      "Initialize your first project from the dashboard.",
      "Invite team members and set their permissions.",
    ],
  },
  {
    title: "Create your first document",
    content: [
      "Open editor and start writing.",
      "Use templates for faster setup.",
      "Add code snippets easily.",
    ],
  },
  {
    title: "Publish & share",
    content: [
      "Review your document.",
      "Publish to your team.",
      "Share public links.",
    ],
  },
];

const next = () => {
  current.value = (current.value + 1) % steps.length;
};

const prev = () => {
  current.value = (current.value - 1 + steps.length) % steps.length;
};
</script>
<template>
  <section
    class="relative py-20 px-6 rounded-2xl overflow-hidden max-w-6xl mx-auto mt-20 mb-20"
    style="
      background-image: url('/pricing_background.png');
      background-size: cover;
    "
  >
    <!-- OVERLAY -->
    <div
      class="absolute inset-0 bg-gradient-to-r from-[#1a1a3d]/80 to-black/80"
    ></div>

    <!-- CONTENT -->
    <div class="relative z-10 text-center">
      <!-- TITLE -->
      <h2 class="text-3xl font-semibold text-white mb-6">Quick Start Guide</h2>

     <div class="flex justify-center items-center gap-2 mb-8">
  <span
    v-for="(step, i) in steps"
    :key="i"
    @click="current = i"
    class="transition-all duration-300 ease-in-out cursor-pointer"
    :class="[
      'rounded-full',
      i === current
        ? 'w-6 h-2 bg-purple-500'
        : 'w-2 h-2 bg-gray-400 hover:bg-gray-300'
    ]"
  />
</div>

      <!-- SLIDER AREA -->
      <div class="flex items-center justify-center gap-6">
        <!-- LEFT ARROW -->
        <button
          @click="prev"
          class="text-white text-2xl opacity-70 hover:opacity-100"
        >
          ‹
        </button>

        <!-- CARD -->
        <div
          class="bg-white/10 backdrop-blur-md border border-white/20 rounded-xl p-6 w-full max-w-xl text-left text-white"
        >
          <div class="flex justify-between items-center mb-3">
            <h3 class="text-lg font-semibold">
              {{ steps[current].title }}
            </h3>
            <span class="text-orange-400 text-sm">
              Step {{ current + 1 }}
            </span>
          </div>

          <ul class="text-sm space-y-2 text-gray-200">
            <li v-for="(item, i) in steps[current].content" :key="i">
              {{ i + 1 }}. {{ item }}
            </li>
          </ul>
        </div>

        <!-- RIGHT ARROW -->
        <button
          @click="next"
          class="text-white text-2xl opacity-70 hover:opacity-100"
        >
          ›
        </button>
      </div>
    </div>
  </section>
</template>
