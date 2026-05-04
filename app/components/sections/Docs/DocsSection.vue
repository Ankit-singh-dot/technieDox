<script setup>
import DocCard from "~/components/ui/DocCard.vue";
</script>

<template>
  <section class="bg-[#EAE9F5] py-20 px-6 pt-36">
    <!-- TITLE -->
    <div class="text-center mb-16">
      <h2 class="text-3xl font-semibold text-[#42389E]">
        Documentation & Guides
      </h2>

      <p class="text-[#868585] mt-3 max-w-xl mx-auto">
        Everything you need to know about building, managing, and scaling your
        knowledge base with TechniDox.
      </p>
    </div>

    <!-- GRID -->
    <div class="max-w-6xl mx-auto grid md:grid-cols-3 gap-6">
      <!-- CARD 1 -->
      <DocCard
        title="Getting Started"
        desc="Learn the basics and set up your account in minutes."
        :items="[
          'Quick Start Guide',
          'Account Setup',
          'Creating Your First Doc',
          'Project Organization',
        ]"
        icon="/star_icon1.png"
        iconBg="bg-[#f2f1ff]"
        bg="bg-white"
      />

      <!-- CARD 2 -->
      <DocCard
        title="Core Features"
        desc="Master the fundamental tools for documentation management."
        :items="[
          'Document Editor',
          'Version Control',
          'Templates Library',
          'Search & Navigation',
        ]"
        icon="/circle_icon1.png"
        iconBg="bg-[#f2f1ff]"
        bg="bg-white"
      />

      <!-- CARD 3 -->
      <DocCard
        title="AI Capabilities"
        desc="Harness the power of AI to automate and improve your docs."
        :items="[
          'AI Writing Assistant',
          'Health Analysis',
          'Automated Summaries',
          'Smart Suggestions',
        ]"
        icon="/user_icon1.png"
        iconBg="bg-[#f2f1ff]"
        bg="bg-white"
      />

      <!-- CARD 4 -->
      <DocCard
        title="Collaboration"
        desc="Work together effectively with your team."
        :items="[
          'Sharing & Permissions',
          'Comments & Feedback',
          'Mentorship System',
          'Community Hub',
        ]"
        icon="/star_icon1.png"
        iconBg="bg-[#f2f1ff]"
        bg="bg-white"
      />

      <!-- CARD 5 -->
      <DocCard
        title="Integrations"
        desc="Connect TechniDox with your existing workflow."
        :items="[
          'GitHub Sync',
          'API Access',
          'Webhook Setup',
          'Slack Integration',
        ]"
        icon="/circle_icon1.png"
        iconBg="bg-[#f2f1ff]"
        bg="bg-white"
      />

      <!-- CARD 6 (SPECIAL BLUE ONE) -->
      <DocCard
        title="Enterprise"
        desc="Advanced tools for large organizations."
        :items="[
          'Team Management',
          'Company Analytics',
          'SSO & Security',
          'Billing & Usage',
        ]"
        icon="/user_icon1.png"
        iconBg="bg-white"
        bg="bg-[#42389E]"
        :dark="true"
      />
    </div>
  </section>
</template>
