<template>
  <div class="cardContainer">
    <div class="imageContainer">
      <img :src="require(`@/assets/${ImageName}`)" alt="pic" />
    </div>
    <div class="textContainer">
      <h2>{{ CardTitle.toUpperCase() }}</h2>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    ImageName: String,
    CardTitle: String,
  },
};
</script>

<style scoped>
.cardContainer {
  position: relative;
  width: 100%;
  height: 650px;
}
.imageContainer img {
  width: 100%;
  height: 100%;
  background-size: cover;
}
.textContainer {
  position: absolute;
  bottom: 0;
  left: 0;
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
