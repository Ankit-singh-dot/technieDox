<template>
  <div
    class="p-6 rounded-xl border border-[#EAE9F5] shadow-sm transition hover:shadow-md"
    :class="bg"
  >
    <!-- ICON -->
    <div
      class="w-10 h-10 flex items-center justify-center rounded-lg mb-4"
      :class="iconBg"
    >
      <img v-if="icon" :src="icon" class="w-5 h-5" />
      <span v-else>✨</span>
    </div>

    <!-- TITLE -->
    <h3
      class="text-lg font-semibold mb-2"
      :class="dark ? 'text-white' : 'text-[#1f1f1f]'"
    >
      {{ title }}
    </h3>

    <!-- DESC -->
    <p class="text-sm mb-4" :class="dark ? 'text-gray-200' : 'text-[#868585]'">
      {{ desc }}
    </p>

    <!-- LIST -->
    <ul class="space-y-2 text-sm">
      <li
        v-for="(item, i) in items"
        :key="i"
        class="flex items-center gap-2"
        :class="dark ? 'text-gray-200' : 'text-[#5d5c5c]'"
      >
        <img
          :src="dark ? '/tick_icon_white.png' : '/tick_icon.png'"
          class="w-4 h-4"
          alt="tick"
        />
        <img
          v-if="status === 'done'"
          :src="dark ? '/tick_icon.png' : '/tick_icon_white.png'"
          class="w-4 h-4"
        />
        {{ item }}
      </li>
    </ul>
  </div>
</template>

<script setup>
defineProps({
  title: String,
  desc: String,
  items: Array,
  icon: String,
  iconBg: String,
  bg: String,
  dark: Boolean,
});
</script>
