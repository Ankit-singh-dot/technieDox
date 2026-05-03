<template>
  <!-- <Navbar /> -->
  <Hero />
  <FeatureSection />
  <AnalyticsSection />
  <PricingPreview />
  <UseCasesSection />
  <CommunitySection />
  <CTAFloating/>
  <FooterSection />
</template>

<script setup>
// import Navbar from "../../components/Navbar.vue";
import AnalyticsSection from "~/components/sections/AnalyticsSection.vue";
import Hero from "../components/sections/Hero.vue";
import FeatureSection from "~/components/sections/FeatureSection.vue";
import PricingPreview from "~/components/sections/PricingPreview.vue";
import UseCasesSection from "~/components/sections/UseCasesSection.vue";
import CommunitySection from "~/components/sections/CommunitySection.vue";
import FooterSection from "~/components/footer/FooterSection.vue";
import CTAFloating from '~/components/sections/Footer/CTAFloating.vue'

</script>
