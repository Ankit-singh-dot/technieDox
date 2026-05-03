<template>
  <nav class="w-full absolute top-0 left-0 z-50">
    <div
      class="max-w-6xl mx-auto px-4 md:px-6 lg:px-8 flex items-center justify-between h-20"
    >

      <div class="flex items-center gap-2">
        <img src="/logo.png" class="h-8" />
        <span class="font-semibold text-purple-700"></span>
      </div>


      <div class="hidden md:flex gap-10">
        <a
          class="text-purple-500 hover:text-purple-700 hover:font-semibold transition"
          >Home</a
        >
        <a
          class="text-purple-500 hover:text-purple-700 hover:font-semibold transition"
          >About Us</a
        >
        <a
          class="text-purple-500 hover:text-purple-700 hover:font-semibold transition"
          >Docs</a
        >
        <a
          class="text-purple-500 hover:text-purple-700 hover:font-semibold transition"
          >Pricing</a
        >
      </div>


      <button class="bg-purple-700 text-white px-5 py-2 rounded-lg">
        Get Started
      </button>
    </div>
  </nav>
</template>
