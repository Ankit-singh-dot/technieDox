# TechnieDox - Modern Landing & Documentation Framework

TechnieDox is a professional-grade landing page and documentation platform built with **Nuxt 4**, **Vue 3**, and **Tailwind CSS**. It provides a high-conversion foundation for developer tools, SaaS products, and technical documentation sites.

##  Overview

This project was developed with a focus on performance, modularity, and clean aesthetics. It features a fully responsive design, custom-built UI components, and a structured layout that guides users from discovery (Hero) to deep-dive (Docs) and finally conversion (Pricing).

##  Architecture & File Structure

The project follows a modular "atomic-to-assembly" architecture:

```text
frontend-assignment/
├── app/
│   ├── components/
│   │   ├── ui/               # Atomic elements (Cards, Buttons, Layout Wrappers)
│   │   ├── sections/         # Feature blocks assembled from UI elements
│   │   ├── Hero/             # specialized assets for the main entry point
│   │   └── Navbar.vue        # Navigation system
│   ├── pages/                # Route-level views (Home, About, Docs, Pricing)
│   └── assets/               # Design tokens and styles
├── nuxt.config.ts            # Framework & Plugin configuration
└── tailwind.config.js        # Design system implementation
```

---

##  Detailed Component Guide

###  Building Blocks (`/ui`)
*   **PricingCard.vue**: A flexible card for subscription tiers. Supports highlighting features and dynamic price points.
*   **DocCard.vue**: Designed for the documentation landing page to showcase categories.
*   **FeatureCard.vue**: standard grid item for showcasing product benefits.
*   **Container.vue**: The architectural backbone of the site, ensuring consistent spacing and max-width across all viewports.

###  Page Sections (`/sections`)
*   **Hero.vue**: The primary visual section with high-impact typography and CTA.
*   **FeatureSection.vue**: Explains the technical advantages of the platform.
*   **AnalyticsSection.vue**: A dedicated space for showcasing metrics and data-driven results.
*   **UseCasesSection.vue**: demonstrates practical applications of the product.
*   **CommunitySection.vue**: Integration points for GitHub, Discord, or other community hubs.

###  Core Pages (`/pages`)
*   **index.vue**: The main entry point, assembling all sections into a cohesive narrative.
*   **docs.vue**: A clean, distraction-free environment for technical reading.
*   **pricing.vue**: detailed comparison of service plans.

---

##  Technology Stack

*   **Nuxt 4**: Next-generation Vue framework for optimal performance and DX.
*   **Tailwind CSS**: Utility-first styling for a custom, premium design system.
*   **Vue 3 (Composition API)**: Modern logic handling for reactive components.
*   **Nuxt Icon**: Unified icon management for a polished UI.

##  Getting Started

1. **Install Dependencies**:
   ```bash
   npm install
   ```

2. **Launch Dev Environment**:
   ```bash
   npm run dev
   ```

3. **Production Build**:
   ```bash
   npm run build
   ```

---

*Handcrafted for VentureSeeds Frontend Assignment.*
