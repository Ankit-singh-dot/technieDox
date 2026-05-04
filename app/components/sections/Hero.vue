<!-- components/sections/Hero.vue -->
<template>
  <section class="grid-bg w-full min-h-[100vh] flex items-center">
    <Navbar />
    <div class="max-w-4xl mx-auto text-center px-4">
      <div class="absolute left-1 top-48 hidden md:inline-block">
        <!-- BACK CARD -->
        <img
          src="/floating_card2.png"
          class="w-[223px] opacity-70 rotate-[8deg] relative z-10 top-28"
        />

        <!-- FRONT CARD -->
        <img
          src="/folating_card1.png"
          class="w-[272px] opacity-90 rotate-[-10deg] absolute top-[-10px] left-[41px] z-20"
        />
      </div>

      <div class="absolute right-5 top-48 hidden md:inline-block">
        <!-- BACK CARD -->
        <img
          src="/floating_card4.png"
          class="w-[223px] opacity-70 rotate-[-8deg] relative z-10 top-40 "
        />

        <!-- FRONT CARD -->
        <img
          src="/floating_card3.png"
          class="w-[272px] opacity-90 rotate-[10deg] absolute top-[-10px] z-20"
        />
      </div>

      <h1 class="text-xl md:text-5xl lg:text-5xl font-bold leading-tight">
        <span class="text-purple-700 italic">Documentation</span>
        that <span class="text-orange-500">builds</span>
        <span class="text-[#5d5c5c]"> itself </span>
        <span class="text-orange-500">improves</span>
        <span class="text-[#5d5c5c]"> itself, and proves its </span>
        <span class="text-orange-500">value</span>
      </h1>
      <p class="mt-6 text-gray-600 text-base md:text-lg max-w-2xl mx-auto">
        AI-native platform that generates documentation from code, scores
        quality in real-time, routes low confidence content to expert review,
        and delivers measurable ROI for enterprise teams.
      </p>

      <div class="mt-8 flex flex-col md:flex-row gap-4 justify-center">
        <button
          class="bg-purple-700 text-white px-6 py-3 rounded-lg shadow hover:bg-purple-800 transition"
        >
          Book a Demo →
        </button>

        <button
          class="border border-purple-300 text-purple-700 px-6 py-3 rounded-lg hover:bg-purple-50 transition"
        >
          Join Enterprise Waitlist
        </button>
      </div>

      <div
        class="mt-8 flex flex-wrap justify-center gap-6 text-sm text-gray-600"
      >
        <span>✔ AI-generated docs in minutes</span>
        <span>✔ Confidence scoring built in</span>
        <span>✔ Enterprise-grade compliance</span>
      </div>
    </div>
  </section>
</template>
