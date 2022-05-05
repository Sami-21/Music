<template>
  <section
    id="Quote"
    class="min-h-screen w-screen flex flex-col justify-center items-center md:px-28 sm:px-16 px-8"
  >
    <div class="lg:w-3/4 w-full mx-auto text-center px-16">
      <p data-aos="fade-down" class="lg:text-6xl md:text-5xl text-4xl">
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quibusdam
        atque sed nam consequatur corrupti.
      </p>
      <h1
        data-aos="fade-up"
        class="lg:text-7xl md:text-6xl text-5xl font-bold mt-16"
      >
        HERBERT SIMON
      </h1>
    </div>
  </section>
</template>

<script>
import AOS from "aos";
import "aos/dist/aos.css"; // You can also use <link> for styles

AOS.init({
  duration: 750,
});
export default {};
</script>

<style>
#Quote {
  background: #ff6309;
  background-image: url(@/assets/featured_image-8.png);
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center center;
  background-blend-mode: multiply;
}
</style>
