<template>
  <main class="min-h-screen w-screen text-white">
    <!-- <NavBar /> -->
    <IntroSection />
    <DanceTourSection />
    <PricingSection />
  </main>
</template>
<script>
// import NavBar from "../components/NavBar.vue";
import IntroSection from "@/components/IntroSection.vue";
import DanceTourSection from "@/components/DanceTourSection.vue";
import PricingSection from "@/components/PricingSection.vue";
// import PriceCard from "../components/PriceCard.vue";
// import StatComponent from "@/components/StatComponent.vue";
export default {
  components: { IntroSection, DanceTourSection, PricingSection },
};
</script>

<style scoped></style>
