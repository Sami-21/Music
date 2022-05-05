<template>
  <section
    id="Stats"
    class="min-h-screen w-screen flex flex-col items-center py-60 md:px-28 sm:px-16 px-0"
  >
    <div data-aos="fade-down" class="lg:w-3/4 w-full mx-auto text-center px-16">
      <h1 class="lg:text-8xl md:text-7xl text-6xl font-bold mb-16">
        OUR STATISTICS
      </h1>
      <p class="lg:text-5xl md:text-4xl text-3xl">
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quibusdam
        atque sed nam consequatur corrupti.
      </p>
    </div>
    <div
      data-aos="fade-up"
      class="w-full grid sm:grid-cols-3 sm:grid-rows-1 grid-cols-1 grid-rows-3 sm:mt-56 mt-20"
    >
      <StatComponent Title="Club" :Digit="1240" />
      <StatComponent Title="Active Member" :Digit="2000" />
      <StatComponent Title="Community" :Digit="1000" />
    </div>
  </section>
</template>

<script>
import AOS from "aos";
import "aos/dist/aos.css"; // You can also use <link> for styles

AOS.init({
  duration: 750,
});

import StatComponent from "./StatComponent.vue";
export default { components: { StatComponent } };
</script>

<style>
#Stats {
  background-color: #2c2c2c;
}
</style>
