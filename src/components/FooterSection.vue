<template>
  <footer
    class="w-screen grid lg:grid-rows-1 lg:grid-cols-2 grid-cols-1 grid-rows-1 sm:pl-16 sm:pb-6 pt-16 md:pt-36"
  >
    <div
      class="h-fit flex flex-col md:justify-start justify-center md:text-left text-center lg:mr-52 px-4"
    >
      <h1 class="xl:text-5xl md:text-4xl text-3xl mb-10 font-bold">
        MUSICOLOGY
      </h1>
      <p class="xl:text-3xl md:text-2xl text-xl mb-8">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit hic
        labore temporibus corporis officiis, aspernatur, atque ad aliquam iste
        similique consequuntur!
      </p>
      <div class="mb-8">
        <v-icon
          class="bg-white p-2 rounded-full mr-4 cursor-pointer"
          size="36px"
          color="#2c2c2c"
          >mdi-instagram</v-icon
        >
        <v-icon
          class="bg-white p-2 rounded-full mr-4 cursor-pointer"
          size="36px"
          color="#2c2c2c"
          >mdi-facebook</v-icon
        >
        <v-icon
          class="bg-white p-2 rounded-full mr-4 cursor-pointer"
          size="36px"
          color="#2c2c2c"
          >mdi-twitter</v-icon
        >
        <v-icon
          class="bg-white p-2 rounded-full mr-4 cursor-pointer"
          size="36px"
          color="#2c2c2c"
          >mdi-whatsapp</v-icon
        >
      </div>
    </div>
    <div
      class="w-full h-full grid sm:grid-cols-3 sm:grid-rows-1 grid-cols-1 grid-rows-3 mx-auto"
    >
      <div
        class="flex flex-col justify-start sm:items-start items-center sm:text-left text-center sm:mb-0 mb-6"
      >
        <h1 class="xl:text-5xl sm:text-4xl text-3xl mb-10 font-bold">ABOUT</h1>
        <ul>
          <li class="xl:text-3xl sm:text-2xl text-lg mb-4">History</li>
          <li class="xl:text-3xl sm:text-2xl text-lg mb-4">Our Team</li>
          <li class="xl:text-3xl sm:text-2xl text-lg mb-4">Brand Guidelines</li>
          <li class="xl:text-3xl sm:text-2xl text-lg mb-4">Terms&Condition</li>
          <li class="xl:text-3xl sm:text-2xl text-lg mb-4">Privacy Policy</li>
        </ul>
      </div>
      <div
        class="flex flex-col justify-start sm:items-start items-center sm:text-left text-center sm:mb-0 mb-6"
      >
        <h1 class="xl:text-5xl sm:text-4xl text-3xl mb-10 font-bold">
          SERVICES
        </h1>
        <ul>
          <li class="xl:text-3xl sm:text-2xl text-lg mb-4">How To Order</li>
          <li class="xl:text-3xl sm:text-2xl text-lg mb-4">Our Product</li>
          <li class="xl:text-3xl sm:text-2xl text-lg mb-4">Order Status</li>
          <li class="xl:text-3xl sm:text-2xl text-lg mb-4">Promo</li>
          <li class="xl:text-3xl sm:text-2xl text-lg mb-4">Payment Method</li>
        </ul>
      </div>
      <div
        class="flex flex-col justify-start sm:items-start items-center sm:text-left text-center"
      >
        <h1 class="xl:text-5xl sm:text-4xl text-3xl mb-10 font-bold">OTHER</h1>
        <ul>
          <li class="xl:text-3xl sm:text-2xl text-lg mb-4">Contact Us</li>
          <li class="xl:text-3xl sm:text-2xl text-lg mb-4">Help</li>
          <li class="xl:text-3xl sm:text-2xl text-lg mb-4">Privacy</li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style>
footer {
  background: #2c2c2c;
  min-height: 600px;
}
@media (min-width: 640px) {
  footer {
    min-height: 0;
  }
}
</style>
