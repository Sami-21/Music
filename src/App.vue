<template>
  <div>
    <HomeView />
  </div>
</template>
<script>
import HomeView from "./Views/HomeView.vue";
export default {
  components: {
    HomeView,
  },
};
</script>
<style>
@import url("https://fonts.googleapis.com/css2?family=Oswald&family=Outfit&display=swap");
@font-face {
  font-family: "Ordax";
  src: url("/home/sami21/.local/share/fonts/Unknown Vendor/TrueType/Ordax/Ordax_Light.ttf");
}

body {
  font-family: "Ordax", "Oswald", sans-serif;
}
</style>
