<template>
  <section id="Subscription" class="w-screen flex justify-center items-center">
    <div class="lg:w-7/12 w-full text-center px-16">
      <h1 class="lg:text-8xl md:text-7xl text-6xl font-bold mb-16">
        SUBSCRIBE
      </h1>
      <p class="lg:text-5xl md:text-4xl text-3xl mb-16">
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quibusdam
        atque sed nam consequatur corrupti.
      </p>
      <form action="" class="mx-auto">
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
          class="w-2/6 py-6 text-xl rounded-tr rounded-br sm:text-3xl outline-0"
        />
      </form>
    </div>
  </section>
</template>

<script>
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
</style>
