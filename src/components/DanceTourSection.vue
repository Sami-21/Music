<template>
  <section
    id="DanceTour"
    class="min-h-screen w-screen flex flex-col items-center py-32 md:px-32 sm:px-16 px-8"
  >
    <img
      src="@/assets/istockphoto-910331794-1024x1024-removebg-preview.png"
      alt="dot"
    />
    <div data-aos="fade-down" class="lg:w-3/4 w-full mx-auto text-center px-16">
      <h1 class="lg:text-8xl md:text-7xl text-6xl font-black mb-16">
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
      <CardComponent CardTitle="AMERICA" ImageName="images.png" />
      <CardComponent CardTitle="ASIA" ImageName="M2.jpeg" />
      <CardComponent CardTitle="AUSTRALIA" ImageName="M1.jpeg" />
    </div>
  </section>
</template>

<script>
import AOS from "aos";
import "aos/dist/aos.css"; // You can also use <link> for styles

AOS.init({
  duration: 750,
});
import CardComponent from "./CardComponent.vue";
export default {
  components: { CardComponent },
};
</script>

<style scoped>
#DanceTour {
  position: relative;
  background: #ff6309;
  overflow: hidden;
}
img {
  position: absolute;
  top: 0;
  left: 0;
  width: 60%;
  height: 60%;
  transform: rotate(5deg) translateX(-20px);
  mask-image: linear-gradient(
    to bottom right,
    rgba(0, 0, 0, 0.6),
    rgba(0, 0, 0, 0),
    rgba(0, 0, 0, 0),
    rgba(0, 0, 0, 0)
  );
}
</style>
