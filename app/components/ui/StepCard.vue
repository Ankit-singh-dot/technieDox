<!-- components/ui/StepCard.vue -->
<template>
  <div
    class="flex items-center justify-between p-4 rounded-lg border border-gray-200 bg-[#f5f4f4]"
  >
    

    <div class="flex items-center gap-3">
      

      <div
        v-if="variant !== 'success'"
        class="w-8 h-8 rounded-full flex items-center justify-center text-sm font-semibold"
        :class="numberBg"
      >
        {{ step }}
      </div>


      <div
        v-else
        class="w-10 h-10 rounded-full flex items-center justify-center bg-green-500 text-white"
      >
        <img src="/tick_fourth.png" alt="">
      </div>


      <div>
        <p class="font-medium text-gray-800">
          {{ title }}
        </p>

        <p class="text-sm text-[#868585]">
          {{ subtitle }}
        </p>
      </div>
    </div>

    <!-- RIGHT SIDE -->
    <div>
      
      <!-- NORMAL STATES -->
      <span
        v-if="variant !== 'success' && status === 'done'"
        class="text-green-500"
      >
        ✔
      </span>

      <span
        v-else-if="variant !== 'success' && status === 'review'"
        class="text-orange-500 text-xs font-medium bg-orange-100 px-2 py-1 rounded"
      >
        Review
      </span>


      <span
        v-if="variant === 'success'"
        class="text-green-500 text-xl"
      >
        ☆
      </span>

    </div>

  </div>
</template>

<script setup>
defineProps({
  step: Number,
  title: String,
  subtitle: String,
  status: String,      
  numberBg: String,    
  variant: String      
})
</script>