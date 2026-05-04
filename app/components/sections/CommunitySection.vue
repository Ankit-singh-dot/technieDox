<!-- components/sections/CommunitySection.vue -->
<template>
  <section class="py-20">
    <!-- HEADER -->
    <div class="text-center max-w-3xl mx-auto px-4">
      <p class="text-orange-500 text-sm uppercase">
        AI-NATIVE DOCUMENTATION ENGINE
      </p>

      <h2 class="mt-2 text-3xl md:text-4xl font-bold text-[#42389E]">
        Community-Driven Improvement At Scale
      </h2>

      <p class="mt-4 text-[#868585]">
        Democratize documentation contributions with gamified workflows,
        micro-tasks, mentorship matching, and peer validation systems that keep
        contributors engaged long-term.
      </p>
    </div>

    <!-- CONTENT -->
    <div class="mt-12 max-w-6xl mx-auto px-4 grid md:grid-cols-2 gap-10">
      <!-- LEFT -->
      <div class="space-y-8">
        <FeatureItem
          title="Gamified Contributions"
          description="Streak tracking, impact badges, and achievement systems that reward quality contributions and retain community members."
          icon="/game_icon.png"
          iconBg="bg-[#f2f1ff]"
        />

        <FeatureItem
          title="Micro-Contribution Architecture"
          description="Complex tasks broken into 5-10 minute contributions, making open source accessible to everyone regardless of time or expertise."
          icon="/micro_icon.png"
          iconBg="bg-[#fef7e8]"
        />

        <FeatureItem
          title="Mentorship Matching"
          description="AI-powered pairing of experienced contributors with newcomers, fostering knowledge transfer and building stronger communities."
          icon="/contro_icon.png"
          iconBg="bg-[#e9f8ea]"
        />

        <FeatureItem
          title="Peer Validation Network"
          description="Accept, edit, and reject workflows that improve AI models over time through community-driven quality signals."
          icon="/perr_icon.png"
          iconBg="bg-[#f2f1ff]"
        />
      </div>

      <!-- RIGHT -->
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

<script setup>
import FeatureItem from "@/components/ui/FeatureItem.vue";
import StepCard from "@/components/ui/StepCard.vue";
</script>
