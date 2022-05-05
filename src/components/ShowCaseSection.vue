<template>
  <section
    id="ShowCase"
    class="w-screen min-h-screen grid grid-cols-1 grid-rows-2 overflow-hidden"
  >
    <div
      class="w-screen min-h-screen grid lg:grid-cols-2 grid-cols-1 lg:grid-rows-1 grid-rows-2"
    >
      <div data-aos="fade-right" class="w-full">
        <img
          id="img1"
          src="@/assets/M1.jpeg"
          alt="M1"
          class="relative w-full h-full lg:right-1 right-0"
        />
      </div>
      <div
        data-aos="fade-left"
        class="w-full h-full lg:text-left text-center flex flex-col justify-center lg:items-start items-center px-24 sm:pt-0 py-8 relative"
      >
        <img
          class="bg-img1 absolute top-0 right-0"
          src="@/assets/istockphoto-910331794-1024x1024-removebg-preview.png"
          alt="dot"
        />
        <img
          class="bg-img2 absolute bottom-0 right-0"
          src="@/assets/istockphoto-910331794-1024x1024-removebg-preview.png"
          alt="dot"
        />
        <h1
          class="lg:text-8xl md:text-7xl sm:text-6xl text-4xl font-bold mb-16"
        >
          AMAZING DANCE
        </h1>
        <p class="lg:text-5xl md:text-4xl sm:text-3xl text-xl mb-24">
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quibusdam
          atque sed nam consequatur corrupti.
        </p>
        <button
          class="md:w-96 w-full h-20 md:text-4xl text-3xl rounded-md font-bold"
        >
          READ MORE
        </button>
      </div>
    </div>
    <div
      class="w-screen min-h-screen grid lg:grid-cols-2 grid-cols-1 lg:grid-rows-1 grid-rows-2"
    >
      <div
        data-aos="fade-right"
        class="w-full h-full lg:text-left text-center flex flex-col justify-center lg:items-start items-center px-24 py-8 lg:order-1 order-2 relative"
      >
        <img
          class="bg-img3 absolute bottom-0 left-0"
          src="@/assets/istockphoto-910331794-1024x1024-removebg-preview.png"
          alt="dot"
        />
        <h1
          class="lg:text-8xl md:text-7xl sm:text-6xl text-4xl font-bold mb-16"
        >
          DANCE BEST
        </h1>
        <p class="lg:text-5xl md:text-4xl sm:text-3xl text-xl mb-24">
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quibusdam
          atque sed nam consequatur corrupti.
        </p>
        <button
          class="md:w-96 w-full h-20 md:text-4xl text-3xl rounded-md font-bold"
        >
          READ MORE
        </button>
      </div>
      <div data-aos="fade-left" class="w-full lg:order-2 order-1">
        <img id="img1" src="@/assets/M2.jpeg" alt="M1" class="w-full h-full" />
      </div>
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

<style scoped>
#ShowCase {
  background: #ff6309;
}
.bg-img1,
.bg-img2,
.bg-img3 {
  height: 60%;
  width: 120%;
  z-index: -1;
}
.bg-img1 {
  transform: rotate(10deg) translate(20px, -70px);
  filter: invert(94%) sepia(94%) saturate(0%) hue-rotate(212deg)
    brightness(107%) contrast(106%);
  opacity: 0.9;
  mask-image: linear-gradient(
    to bottom left,
    rgba(0, 0, 0, 0.6),
    rgba(0, 0, 0, 0),
    rgba(0, 0, 0, 0)
  );
}
.bg-img2 {
  transform: rotate(15deg) translateX(25px, 50px) !important;

  filter: invert(94%) sepia(94%) saturate(0%) hue-rotate(212deg)
    brightness(107%) contrast(106%);

  mask-image: linear-gradient(
    to top left,
    rgba(0, 0, 0, 0.6),
    rgba(0, 0, 0, 0),
    rgba(0, 0, 0, 0),
    rgba(0, 0, 0, 0)
  );
}
.bg-img3 {
  transform: rotate(90deg) translateX(25px, 0px) !important;
  filter: invert(94%) sepia(94%) saturate(0%) hue-rotate(212deg)
    brightness(107%) contrast(106%);

  mask-image: linear-gradient(
    to top right,
    rgba(0, 0, 0, 0.6),
    rgba(0, 0, 0, 0),
    rgba(0, 0, 0, 0)
  );
}

button {
  background: #2c2c2c;
}
</style>
