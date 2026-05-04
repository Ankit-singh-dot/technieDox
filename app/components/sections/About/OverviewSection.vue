<script setup>
import StepCard from "~/components/ui/StepCard.vue";
</script>

<template>
  <section class="bg-[#] py-20 px-6 min-h-screen h-full mt-7">
    <!-- TITLE -->
    <h2 class="text-center text-3xl font-semibold text-[#42389E] mb-16">
      TechniDox Overview
    </h2>

    <!-- GRID -->
    <div class="max-w-6xl mx-auto grid md:grid-cols-2 gap-12 items-start pt-10">
      <!-- LEFT SIDE -->
      <div>
        <p class="text-[#868585] leading-relaxed mb-6">
          TechniDox is an enterprise-grade knowledge infrastructure platform
          designed to transform how teams create, manage, and scale their
          documentation.
        </p>

        <p class="text-[#868585] leading-relaxed mb-6">
          By combining AI-powered insights with collaborative workflows,
          TechniDox ensures your organizational knowledge is always accurate,
          accessible, and up-to-date.
        </p>

        <!-- FEATURES -->
        <ul class="space-y-3 text-[#5d5c5c]">
          <li class="flex items-center gap-2">
            <span class="text-[#42389E]">✔</span>
            AI-Powered Writing Assistant
          </li>

          <li class="flex items-center gap-2">
            <span class="text-[#42389E]">✔</span>
            Real-time Health Analysis
          </li>

          <li class="flex items-center gap-2">
            <span class="text-[#42389E]">✔</span>
            Enterprise Security
          </li>

          <li class="flex items-center gap-2">
            <span class="text-[#42389E]">✔</span>
            Cross-Team Collaboration
          </li>
        </ul>
      </div>

      <!-- RIGHT SIDE -->
      <div class="bg-white p-6 rounded-xl border border-gray-200 space-y-4">
        <StepCard
          :step="1"
          title="AI generates documentation"
          subtitle="From codebase analysis"
          status="done"
          numberBg="bg-purple-100 text-purple-700"
        />

        <StepCard
          :step="2"
          title="Quality scoring & routing"
          subtitle="Confidence: 72% - Review needed"
          status="review"
          numberBg="bg-orange-100 text-orange-600"
        />

        <StepCard
          :step="3"
          title="Community review"
          subtitle="3 contributors validated"
          status="done"
          numberBg="bg-green-100 text-green-600"
        />

        <StepCard
          :step="4"
          variant="success"
          title="Published & improving"
          subtitle="AI learns from feedback"
          status="idle"
          numberBg="bg-green-500 text-white"
        />
      </div>
    </div>
  </section>
</template>
