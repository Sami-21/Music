<template>
  <section
    id="IntroSection"
    class="relative min-h-screen w-screen flex items-end py-16 sm:px-28 px-14"
  >
    <div class="xl:w-1/2 lg:my-0 w-full lg:text-left text-center my-auto">
      <h1 class="lg:text-9xl md:text-8xl text-7xl">Title Here</h1>
      <p class="lg:text-5xl md:text-4xl text-3xl mt-14">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Aspernatur
        ratione eius numquam maxime distinctio.
      </p>
      <button
        class="sm:px-28 sm:py-5 mt-14 sm:text-3xl py-4 px-24 text-xl rounded"
      >
        REGISTER NOW
      </button>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
#IntroSection {
  background-image: url(../assets/featured_image-8.png);
  background-position: center center;
  background-repeat: no-repeat;
  background-size: cover;
}

#IntroSection button {
  background: #ff6309;
}
</style>
