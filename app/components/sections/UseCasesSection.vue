<!-- app/components/sections/UseCasesSection.vue -->
<template>
  <section class="py-20">

    <div class="text-center max-w-3xl mx-auto px-4">
      <p class="text-orange-500 text-sm uppercase">USE CASES</p>

      <h2 class="mt-2 text-3xl md:text-4xl font-bold text-[#42389E]">
        Built For Every Team That Ships Code.
      </h2>

      <p class="mt-4 text-[#868585]">
        Whether you're a solo OSS maintainer or a 10,000-person enterprise,
        TechniDox adapts to how your team creates and maintains documentation.
      </p>
    </div>


    <div class="mt-12 max-w-6xl mx-auto px-4 grid md:grid-cols-2 gap-6">

      <UseCaseCard
        label="Open Source Teams"
        title="Ship docs as fast as you ship code"
        description="Democratize contributions with micro-tasks, voice input, and mentorship matching. Keep your community engaged with gamification that makes documentation feel like progress, not chores."
        :points="[
          '78% less burden on maintainers',
          'Non-technical contributors via micro-tasks',
          'Gamified streaks keep contributors returning',
        ]"
        icon="/raphael_opensource.png"
        iconBg="bg-[#f2f1ff]"
      />


      <UseCaseCard
        label="Engineering Enablement"
        title="Onboard developers 2.3x faster"
        description="Connect your CI/CD pipeline to TechniDox and auto-generate docs on every merge. Quality gates catch regressions before they reach production. Developers self-serve answers instead of interrupting colleagues."
        :points="[
          'CI/CD quality gates prevent doc regressions',
          'Auto-generated docs on every merge',
          '34% fewer interruptions',
        ]"
        icon="/Vector.png"
        iconBg="bg-[#fef7e8]"
      />


      <UseCaseCard
        label="Platform Teams"
        title="Documentation that scales with your APIs"
        description="Generate API reference docs, SDK guides, and integration playbooks automatically from your codebase. Keep them in sync with confidence scoring that flags drift before your customers notice."
        :points="[
          'Auto-synced API reference',
          'Multi-format export',
          'Confidence alerts in real time',
        ]"
        icon="/Vector (1).png"
        iconBg="bg-[#e9f8ea]"
      />


      <UseCaseCard
        label="Enterprise Documentation" 
        title="Documentation your auditors will approve"
        description="Meet ISO, SOC2, and internal compliance requirements with automated audit trails, version control, and executive dashboards. Show documentation ROI to the C-suite with numbers that matter."
        :points="[
          'ISO 27001 & SOC2 compliance',
          'Full audit trail',
          'Executive ROI dashboards',
        ]"
        icon="/box.png"
        iconBg="bg-[#f2f1ff]"
        bgClass="bg-[#42389E] text-white"
      />
    </div>
  </section>
</template>

<script setup>
import UseCaseCard from "@/components/ui/UseCaseCard.vue";
</script>
