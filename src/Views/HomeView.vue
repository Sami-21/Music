<template>
  <main class="min-h-screen w-screen text-white">
    <NavBar />
    <IntroSection />
    <DanceTourSection />
    <PricingSection />
    <ShowCaseSection />
    <StatsSection />
    <section
      id="Quote"
      class="min-h-screen w-screen flex flex-col justify-center items-center md:px-28 sm:px-16 px-8"
    >
      <div class="lg:w-3/4 w-full mx-auto text-center px-16">
        <p class="lg:text-6xl md:text-5xl text-4xl">
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quibusdam
          atque sed nam consequatur corrupti.
        </p>
        <h1 class="lg:text-7xl md:text-6xl text-5xl font-bold mt-16">
          HERBERT SIMON
        </h1>
      </div>
    </section>
  </main>
</template>
<script>
import NavBar from "../components/NavBar.vue";
import IntroSection from "@/components/IntroSection.vue";
import DanceTourSection from "@/components/DanceTourSection.vue";
import PricingSection from "@/components/PricingSection.vue";
import ShowCaseSection from "@/components/ShowCaseSection.vue";
import StatsSection from "@/components/StatsSection.vue";

// import StatComponent from "@/components/StatComponent.vue";
export default {
  components: {
    NavBar,
    IntroSection,
    DanceTourSection,
    PricingSection,
    ShowCaseSection,
    StatsSection,
  },
};
</script>

<style scoped>
#Quote {
  background: #ff6309;
  background-image: url(@/assets/featured_image-8.png);
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center center;
  background-blend-mode: multiply;
}
</style>
