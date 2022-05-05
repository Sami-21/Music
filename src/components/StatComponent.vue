<template>
  <div class="w-full text-center mb-20">
    <h1 class="lg:text-7xl md:text-6xl text-5xl font-bold mb-8">
      {{ (Digit / 1000).toFixed(3) }}+
    </h1>
    <h1 class="lg:text-5xl md:text-4xl text-3xl">{{ Title }}</h1>
  </div>
</template>

<script>
export default {
  props: {
    Title: String,
    Digit: Number,
  },
};
</script>

<style scoped></style>
