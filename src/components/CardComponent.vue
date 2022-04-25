<template>
  <div class="cardContainer">
    <div class="imageContainer"></div>
    <div class="textContainer">
      <h2>{{ CardTitle.toUpperCase() }}</h2>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    ImageURL: String,
    CardTitle: String,
  },
  computed: {
    image() {
      return `background:url(${this.ImageURL})`;
    },
  },
};
</script>

<style scoped>
.cardContainer {
  width: 100%;
  height: 650px;
}
.imageContainer {
  width: 100%;
  height: 400px;
  background: url("../assets/images.png");
  background-size: cover;
}
.textContainer {
  padding-top: 30px;
  width: 100%;
  height: 250px;
  background: #2c2c2c;
  text-align: center;
}
.textContainer h2 {
  font-size: 48px;
}
.textContainer p {
  font-size: 36px;
}
</style>
