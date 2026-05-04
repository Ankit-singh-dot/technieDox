<template>
  <section class="bg-[#f5f4f4] py-20 px-6">

    <div class="text-center max-w-3xl mx-auto mb-10">
      <p class="text-xs text-orange-500 uppercase tracking-wider mb-2">
        WHY TECHNIDOX
      </p>

      <h2 class="text-3xl font-semibold text-[#42389E]">
        Not Just Another Documentation Tool
      </h2>

      <p class="text-sm text-[#868585] mt-3">
        Traditional tools give you a place to write. TechniDox gives you a
        system that generates, scores, validates, and continuously improves
        documentation.
      </p>
    </div>


    <div
      class="max-w-6xl mx-auto overflow-hidden rounded-xl border border-gray-200"
    >

      <div
        class="grid grid-cols-[2fr_1fr_1fr] bg-[#4b3fa7] text-white text-sm font-medium"
      >
        <div class="p-4">Capability</div>
        <div class="p-4 text-center">TechniDox</div>
        <div class="p-4 text-center">Traditional Documentation</div>
      </div>


      <div
        v-for="(row, i) in rows"
        :key="i"
        class="grid grid-cols-[2fr_1fr_1fr] border-t border-gray-200 text-sm"
        :class="[
          i % 2 === 0 ? 'bg-white' : 'bg-[#fafafa]',
          'hover:bg-gray-50 transition',
        ]"
      >

        <div class="p-4 text-gray-700  border-r border-gray-300">
          {{ row.name }}
        </div>


        <div class="p-4 flex justify-center  border-r border-gray-300">
          <span v-if="row.tech" class="text-green-500">✔</span>
          <span v-else>—</span>
        </div>


        <div class="p-4 flex justify-center">
          <span v-if="row.traditional" class="text-green-500">✔</span>
          <span v-else>—</span>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const rows = [
  { name: "AI-native architecture", tech: true, traditional: false },
  { name: "Confidence scoring per doc", tech: true, traditional: false },
  {
    name: "Multi-dimensional quality assessment",
    tech: true,
    traditional: false,
  },
  {
    name: "Human-in-the-loop review workflows",
    tech: true,
    traditional: false,
  },
  { name: "Gamified community contributions", tech: true, traditional: false },
  { name: "Real-time ROI dashboard", tech: true, traditional: false },
  { name: "ISO / SOC2 compliance reporting", tech: true, traditional: false },
  { name: "CI/CD quality gate integration", tech: true, traditional: false },
  { name: "Basic markdown editing", tech: true, traditional: true },
  { name: "Team collaboration", tech: true, traditional: true },
];
</script>
