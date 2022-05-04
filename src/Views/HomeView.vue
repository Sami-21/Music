<template>
  <main class="min-h-screen w-screen text-white">
    <NavBar />
    <section
      id="IntroSection"
      class="relative min-h-screen w-screen flex items-end py-16 px-28"
    >
      <div class="md:w-1/2">
        <h1 class="block text-9xl">Title Here</h1>
        <p class="block text-4xl">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Aspernatur
          ratione eius numquam maxime distinctio.
        </p>
        <button class="block">REGISTER NOW</button>
      </div>
    </section>
  </main>
</template>
<script>
import NavBar from "../components/NavBar.vue";
// import Card from "../components/CardComponent.vue";
// import PriceCard from "../components/PriceCard.vue";
// import StatComponent from "@/components/StatComponent.vue";
export default {
  components: { NavBar },
};
</script>

<style scoped>
#IntroSection {
  background-image: url(../assets/featured_image-8.png);
  background-position: center center;
  background-repeat: no-repeat;
  background-size: cover;
}
#IntroSection div {
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
#IntroSection button {
  background: #ff6309;
}
</style>
