<!-- components/ui/FeatureItem.vue -->
<template>
  <div class="flex gap-4">
    <!-- ICON -->
    <div
      class="w-10 h-10 rounded-lg flex items-center justify-center"
      :class="iconBg"
    >
      <img :src="icon" class="w-5 h-5" />
    </div>

    <!-- TEXT -->
    <div>
      <h3 class="text-lg font text-black">
        {{ title }}
      </h3>

      <p class="mt-1 text-sm text-[#868585] max-w-md">
        {{ description }}
      </p>
    </div>
  </div>
</template>

<script setup>
defineProps({
  title: String,
  description: String,
  icon: String,
  iconBg: String,
});
</script>
