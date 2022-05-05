<template>
  <main class="min-h-screen w-screen text-white">
    <NavBar />
    <IntroSection />
    <DanceTourSection />
    <PricingSection />
    <ShowCaseSection />
  </main>
</template>
<script>
import NavBar from "../components/NavBar.vue";
import IntroSection from "@/components/IntroSection.vue";
import DanceTourSection from "@/components/DanceTourSection.vue";
import PricingSection from "@/components/PricingSection.vue";
import ShowCaseSection from "@/components/ShowCaseSection.vue";
// import StatComponent from "@/components/StatComponent.vue";
export default {
  components: {
    NavBar,
    IntroSection,
    DanceTourSection,
    PricingSection,
    ShowCaseSection,
  },
};
</script>

<style scoped></style>
