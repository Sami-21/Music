<template>
  <section
    id="Subscription"
    class="w-screen flex justify-center items-center relative overflow-hidden"
  >
    <img
      src="@/assets/istockphoto-910331794-1024x1024-removebg-preview.png"
      alt="dot"
      class="absolute top-0 left-0 h-full w-4/6 rotate-12 -translate-x-20 -translate-y-4 img1"
    />
    <img
      src="@/assets/istockphoto-910331794-1024x1024-removebg-preview.png"
      alt="dot"
      class="absolute bottom-0 right-0 h-full w-4/6 rotate-12 translate-x-20 translate-y-4 img2"
    />
    <div class="lg:w-7/12 w-full text-center px-16">
      <h1
        data-aos="fade-right"
        class="lg:text-8xl md:text-7xl text-6xl font-bold mb-16"
      >
        SUBSCRIBE
      </h1>
      <p data-aos="fade-right" class="lg:text-5xl md:text-4xl text-3xl mb-16">
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quibusdam
        atque sed nam consequatur corrupti.
      </p>
      <form action="" class="mx-auto" data-aos="fade-left">
        <input
          class="w-4/6 p-6 bg-white text-xl sm:text-3xl outline-0 text-black"
          type="email"
          name="email"
          id="email"
          placeholder="Your Email"
        />
        <input
          type="submit"
          id="subscribe"
          value="SUBSCRIBE"
          class="w-2/6 py-6 text-lg rounded-tr rounded-br sm:text-3xl outline-0 font-bold"
        />
      </form>
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
#Subscription {
  background: #ff6309;
  height: 700px;
}
#id {
  color: #2c2c2c;
}
#subscribe {
  background: #2c2c2c;
}
.img1,
.img2 {
  height: 150%;
  filter: invert(15%) sepia(0%) saturate(0%) hue-rotate(5deg) brightness(98%)
    contrast(92%);
}
.img1 {
  mask-image: linear-gradient(
    to right,
    rgba(0, 0, 0, 0.6),
    rgba(0, 0, 0, 0),
    rgba(0, 0, 0, 0)
  );
}
.img2 {
  mask-image: linear-gradient(
    to left,
    rgba(0, 0, 0, 0.6),
    rgba(0, 0, 0, 0),
    rgba(0, 0, 0, 0)
  );
}
</style>
