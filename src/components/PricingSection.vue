<template>
  <section
    id="Pricing"
    class="min-h-screen w-screen flex flex-col items-center py-32 md:px-32 sm:px-16 px-12 relative"
  >
    <img
      src="@/assets/istockphoto-910331794-1024x1024-removebg-preview.png"
      alt="dot"
    />
    <img
      src="@/assets/istockphoto-910331794-1024x1024-removebg-preview.png"
      alt="dot"
    />
    <div
      data-aos="fade-down"
      class="lg:w-3/4 w-full mx-auto text-center sm:px-16 px-8"
    >
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
import AOS from "aos";
import "aos/dist/aos.css"; // You can also use <link> for styles

AOS.init({
  duration: 750,
});
import PriceCard from "./PriceCard.vue";
export default { components: { PriceCard } };
</script>

<style scoped>
#Pricing {
  background-color: #2c2c2c;
  overflow: hidden;
}
img {
  position: absolute;
  width: 60%;
  height: 60%;
}
img:nth-child(1) {
  transform: rotate(-4deg) translate(20px, -30px);
  top: 0;
  left: 0;
  filter: invert(29%) sepia(5%) saturate(6%) hue-rotate(4deg) brightness(92%)
    contrast(83%);
  mask-image: linear-gradient(
    to bottom right,
    rgba(0, 0, 0, 0.5),
    rgba(0, 0, 0, 0),
    rgba(0, 0, 0, 0),
    rgba(0, 0, 0, 0)
  );
}
img:nth-child(2) {
  bottom: 0;
  right: 0;
  transform: rotate(10deg) translate(20px, 30px);
  filter: invert(39%) sepia(11%) saturate(17%) hue-rotate(327deg)
    brightness(94%) contrast(84%);

  mask-image: linear-gradient(
    to top left,
    rgba(0, 0, 0, 0.6),
    rgba(0, 0, 0, 0),
    rgba(0, 0, 0, 0),
    rgba(0, 0, 0, 0)
  );
}
</style>
