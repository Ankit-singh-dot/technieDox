<template>
  <div
    class="rounded-xl p-6 border border-gray-200  flex gap-4"
    :class="bgClass"
  >

    <div
      class="w-12 h-12 flex items-center justify-center rounded-lg"
      :class="iconBg"
    >
      <img :src="icon" class="w-6 h-6" />
    </div>


    <div>
      <p class="text-xs font-medium text-gray-500 uppercase"
      :class="bgClass ? 'text-white' : 'text-[#42389E]'">
        {{ label }}
      </p>

      <h3
        class="text-lg font-normal mt-1 text-[#42389E]"
        :class="bgClass ? 'text-white' : 'text-black'"
      >
        {{ title }}
      </h3>

      <p
        class="mt-2 text-sm text-[#868585] max-w-md"
        :class="bgClass ? 'text-white/80' : 'text-[#868585]'"
      >
        {{ description }}
      </p>


      <ul
        class="mt-4 space-y-2 text-sm text-[#5d5c5c]"
        :class="bgClass ? 'text-white/90' : 'text-[#5d5c5c]'"
      >
        <li
          v-for="(item, i) in points"
          :key="i"
          class="flex items-center gap-2"
        >
          <span class="text-green-500">✔</span>
          {{ item }}
        </li>
      </ul>
    </div>
  </div>
</template>

<script setup>
defineProps({
  label: String,
  title: String,
  description: String,
  points: Array,
  icon: String,
  iconBg: String,
  bgClass: String,
});
</script>
