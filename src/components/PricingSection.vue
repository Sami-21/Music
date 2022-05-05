<template>
  <section
    id="Pricing"
    class="min-h-screen w-screen flex flex-col items-center py-32 md:px-32 sm:px-16 px-12"
  >
    <div class="lg:w-3/4 w-full mx-auto text-center px-16">
      <h1 class="lg:text-8xl md:text-7xl text-6xl font-bold mb-16">PRICING</h1>
      <p class="lg:text-4xl md:text-3xl text-2xl">
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quibusdam
        atque sed nam consequatur corrupti.
      </p>
    </div>
    <div
      class="grid gap-20 xl:grid-cols-3 lg:grid-cols-2 grid-cols-1 w-full min-h-fit mt-24"
    >
      <PriceCard BundleName="BASIC" :BundlePrice="150" />
      <PriceCard BundleName="PROFESSIONAL" :BundlePrice="200" />
      <PriceCard BundleName="ULTIMATE" :BundlePrice="250" />
    </div>
  </section>
</template>

<script>
import PriceCard from "./PriceCard.vue";
export default { components: { PriceCard } };
</script>

<style>
#Pricing {
  background-color: #2c2c2c;
}
</style>
