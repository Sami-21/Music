<template>
  <div class="statElement">
    <h1>{{ Digit }}+</h1>
    <h1>{{ Title }}</h1>
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

<style scoped>
.statElement {
  width: 1fr;
  height: fit-content;
  text-align: center;
}
.statElement h1 {
  font-size: 72px;
}
.statElement h1:nth-child(2) {
  font-weight: 100;
}
</style>
