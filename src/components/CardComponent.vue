<template>
  <div data-aos="fade-down" id="CardContainer" class="w-full relative">
    <div class="w-full h-full bg-white">
      <img
        :src="require(`@/assets/${ImageName}`)"
        alt="pic"
        class="w-full h-full"
      />
    </div>
    <div
      id="textContainer"
      class="absolute bottom-0 left-0 w-full h-52 text-center py-8 px-6"
    >
      <h2 class="xl:text-5xl lg:text-4xl md:text-3xl text-2xl mb-4">
        {{ CardTitle.toUpperCase() }}
      </h2>
      <p class="lg:text-2xl md:text-xl text-lg">
        Lorem ipsum dolor sit amet consectetur adipisicing elit.
      </p>
    </div>
  </div>
</template>

<script>
import AOS from "aos";
import "aos/dist/aos.css"; // You can also use <link> for styles

AOS.init();
export default {
  props: {
    ImageName: String,
    CardTitle: String,
  },
};
</script>

<style scoped>
#CardContainer {
  height: 615px;
}

#textContainer {
  background: #2c2c2c;
}
</style>
