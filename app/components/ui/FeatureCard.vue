<template>
  <div
    class="p-6 rounded-xl border shadow-sm flex-row gap-6 items-start flex"
    :class="
      dark
        ? 'bg-[#42389E] text-white border-transparent'
        : 'bg-white border-gray-200'
    "
  >
    <!-- ICON -->
    <div
      class="w-24 h-10 flex items-center justify-center rounded-lg"
      :class="dark ? 'bg-white' : 'bg-[#f2f1ff]'"
    >
      <img :src="icon" class="w-5 h-5" />
    </div>

    <!-- TEXT -->
    <div>
      <h3 class="text-lg font-semibold mb-1">
        {{ title }}
      </h3>

      <p class="text-sm" :class="dark ? 'text-gray-200' : 'text-[#868585]'">
        {{ desc }}
      </p>
    </div>
  </div>
</template>

<script setup>
defineProps({
  title: String,
  desc: String,
  icon: String,
  dark: Boolean,
});
</script>
