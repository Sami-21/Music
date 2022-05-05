<template>
  <main class="min-h-screen w-screen text-white">
    <NavBar />
    <IntroSection />
    <DanceTourSection />
    <PricingSection />
    <ShowCaseSection />
    <StatsSection />
    <QuoteSection />
    <SubscriptionSection />
  </main>
</template>
<script>
import NavBar from "../components/NavBar.vue";
import IntroSection from "@/components/IntroSection.vue";
import DanceTourSection from "@/components/DanceTourSection.vue";
import PricingSection from "@/components/PricingSection.vue";
import ShowCaseSection from "@/components/ShowCaseSection.vue";
import StatsSection from "@/components/StatsSection.vue";
import QuoteSection from "../components/QuoteSection.vue";
import SubscriptionSection from "../components/SubscriptionSection.vue";

// import StatComponent from "@/components/StatComponent.vue";
export default {
  components: {
    NavBar,
    IntroSection,
    DanceTourSection,
    PricingSection,
    ShowCaseSection,
    StatsSection,
    QuoteSection,
    SubscriptionSection,
  },
};
</script>

<style scoped></style>
