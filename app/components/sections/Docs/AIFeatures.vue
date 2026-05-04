<script setup>
import FeatureCard from "~/components/ui/FeatureCard.vue";
</script>

<template>
  <section class="bg-[#f5f4f4] py-20 px-6">
    <div class="max-w-6xl mx-auto grid md:grid-cols-3 gap-6 items-stretch">
      <!-- LEFT TEXT -->
      <div class="flex flex-col justify-center">
        <h2 class="text-3xl font-semibold text-[#42389E] mb-4">
          AI-Powered Features
        </h2>

        <p class="text-[#5d5c5c] max-w-sm leading-relaxed">
          TechniDox leverages advanced machine learning to automate the tedious
          parts of documentation.
        </p>
      </div>


      <FeatureCard
        title="Clarity Engine"
        desc="Automatically analyzes your text for readability, technical accuracy, and tone consistency."
        icon="/clarity_icon.png"
        ,
      />


      <FeatureCard
        title="Smart Sync"
        desc="Keeps your docs in sync with your codebase by automatically detecting changes in GitHub repositories."
        icon="/os_icon.png"
        :dark="true"
      />
    </div>
  </section>
</template>
