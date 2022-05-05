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
    <FooterSection />
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
import FooterSection from "@/components/FooterSection.vue";

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
    FooterSection,
  },
};
</script>

<style scoped>
main {
  overflow-x: hidden;
}
</style>
