<template>
  <div class="cardContainer">
    <div class="textContainer">
      <div class="iconContainer">
        <h1>Icon</h1>
      </div>
      <h2>{{ BundleName.toUpperCase() }}</h2>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
      <button>${{ BundlePrice }}.00</button>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    BundleName: String,
    BundlePrice: Number,
  },
};
</script>

<style scoped>
.cardContainer {
  width: 100%;
  height: 650px;
  background-color: #ff6309;
  border-radius: 10px;
}

.textContainer {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  padding: 30px;
  width: 100%;
  height: 100%;
  text-align: center;
}
.iconContainer {
  width: 100%;
  height: 300px;
  background-color: black;
}
.textContainer h2 {
  font-size: 48px;
}
.textContainer p {
  font-size: 36px;
}
.textContainer button {
  width: 100%;
  padding: 15px;
  font-size: 36px;
  background: #2c2c2c;
  border-radius: 5px;
}
</style>
