<template>
  <section id="ShowCase" class="w-screen min-h-screen">
    <div
      class="w-screen min-h-screen grid lg:grid-cols-2 grid-cols-1 lg:grid-rows-1 grid-rows-2"
    >
      <div class="w-full">
        <img
          id="img1"
          src="@/assets/M1.jpeg"
          alt="M1"
          class="relative w-full h-full lg:right-1 right-0"
        />
      </div>
      <div
        class="w-full h-full lg:text-left text-center flex flex-col justify-center lg:items-start items-center px-24"
      >
        <h1 class="lg:text-8xl md:text-7xl text-6xl font-bold mb-16">
          AMAZING DANCE
        </h1>
        <p class="lg:text-5xl md:text-4xl text-3xl mb-24">
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quibusdam
          atque sed nam consequatur corrupti.
        </p>
        <button class="w-96 h-20 md:text-4xl text-3xl rounded-md">
          READ MORE
        </button>
      </div>
    </div>
    <div
      class="w-screen min-h-screen grid lg:grid-cols-2 grid-cols-1 lg:grid-rows-1 grid-rows-2"
    >
      <div
        class="w-full h-full lg:text-left text-center flex flex-col justify-center lg:items-start items-center px-24 lg:order-1 order-2"
      >
        <h1 class="lg:text-8xl md:text-7xl text-6xl font-bold mb-16">
          DANCE BEST
        </h1>
        <p class="lg:text-5xl md:text-4xl text-3xl mb-24">
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quibusdam
          atque sed nam consequatur corrupti.
        </p>
        <button class="w-96 h-20 md:text-4xl text-3xl rounded-md">
          READ MORE
        </button>
      </div>
      <div class="w-full lg:order-2 order-1">
        <img id="img1" src="@/assets/M2.jpeg" alt="M1" class="w-full h-full" />
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
#ShowCase {
  background: #ff6309;
}
button {
  background: #2c2c2c;
}
</style>
