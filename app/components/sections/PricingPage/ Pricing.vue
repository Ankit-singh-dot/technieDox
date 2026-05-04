<script setup>

import PricingCard from "~/components/ui/PricingCard.vue";
</script>

<template>
  <section
    class="relative min-h-screen b bg-center"
    style="background-image: url('/pricing_background.png')"
  >
    <!-- NAVBAR -->
    

    <!-- CONTENT -->
    <div class="pt-32 pb-20 px-6">
      <!-- TITLE -->
      <div class="text-center mb-12">
        <h2 class="text-white text-3xl md:text-4xl font-semibold">
          Plans Built For Every Stage Of Growth
        </h2>
      </div>

      <!-- CARDS -->
      <div class="max-w-6xl mx-auto grid md:grid-cols-3 gap-6">
        <PricingCard
          title="Standard"
          price="499"
          :features="[
            'AI Documentation Assistant',
            'Team Collaboration',
            'Basic Analytics',
            '5GB Storage',
            'Email Support',
            'Standard Templates',
            'Public API Access',
          ]"
        />

        <PricingCard
          title="Enhanced"
          price="1499"
          highlight
          badge="Popular"
          :features="[
            'Everything in Starter',
            'Advanced AI Features',
            'SSO Integration',
            'Advanced Analytics',
            '50GB Storage',
            'Priority Support',
            'Custom Branding',
          ]"
        />

        <PricingCard
          title="Enterprise"
          custom
          :features="[
            'Everything in Growth',
            'Custom Integration',
            'Dedicated Support',
            'Custom AI Training',
            'Unlimited Storage',
            '24/7 Premium Support',
            'SLA Guarantee',
          ]"
        />
      </div>
    </div>
  </section>
</template>
