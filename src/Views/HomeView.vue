<template>
  <main class="min-h-screen w-screen text-white">
    <!-- <NavBar /> -->
    <IntroSection />
    <section
      id="DanceTour"
      class="min-h-screen w-screen flex flex-col items-center py-32 md:px-32 sm:px-16 px-8"
    >
      <div class="lg:w-1/2 w-full mx-auto text-center px-16">
        <h1 class="lg:text-8xl md:text-7xl text-6xl font-bold mb-16">
          DANCE TOUR
        </h1>
        <p class="lg:text-4xl md:text-3xl text-2xl">
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quibusdam
          atque sed nam consequatur corrupti.
        </p>
      </div>
      <div
        class="grid gap-20 xl:grid-cols-3 lg:grid-cols-2 grid-cols-1 w-full min-h-fit mt-24"
      >
        <CardComponent CardTitle="ASIA" />
        <CardComponent CardTitle="AMERICA" />
        <CardComponent CardTitle="AUSTRALIA" />
      </div>
    </section>
  </main>
</template>
<script>
// import NavBar from "../components/NavBar.vue";
import IntroSection from "@/components/IntroSection.vue";
import CardComponent from "@/components/CardComponent.vue";
// import Card from "../components/CardComponent.vue";
// import PriceCard from "../components/PriceCard.vue";
// import StatComponent from "@/components/StatComponent.vue";
export default {
  components: { IntroSection, CardComponent },
};
</script>

<style scoped>
#DanceTour {
  background: #ff6309;
}
</style>
