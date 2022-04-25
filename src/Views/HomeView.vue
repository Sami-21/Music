<template>
  <div class="home">
    <NavBar></NavBar>
    <section id="IntroSection">
      <div class="contentContainer" id="IntroSectionContainer">
        <div class="TextBox">
          <h1>Title Here</h1>
          <p>
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Delectus
            hic praesentium quibusdam quisquam mollitia.
          </p>
          <button id="register-btn">REGISTER NOW</button>
        </div>
      </div>
    </section>

    <section id="DanceTour">
      <div class="contentContainer">
        <div class="textContainer">
          <h1>DANCE TOUR</h1>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi nobis
            quis aliquid similique, repellendus tenetur eos!
          </p>
        </div>
        <div class="cardsContainer">
          <Card CardTitle="america" imageURL="../assets/images.png"></Card>
          <Card CardTitle="asia" imageURL="../assets/images.png"></Card>
          <Card CardTitle="australia" imageURL="../assets/images.png"></Card>
        </div>
      </div>
    </section>

    <section id="Pricing">
      <div class="contentContainer">
        <div class="textContainer">
          <h1>PRICING</h1>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Deleniti
            fugiat numquam totam, possimus esse distinctio illo?
          </p>
        </div>
        <div class="cardsContainer">
          <PriceCard BundleName="Basic" v-bind:BundlePrice="100"></PriceCard>
          <PriceCard
            BundleName="professional"
            v-bind:BundlePrice="150"
          ></PriceCard>
          <PriceCard BundleName="ultimate" v-bind:BundlePrice="250"></PriceCard>
        </div>
      </div>
    </section>
  </div>
</template>
<script>
import NavBar from "../components/NavBar.vue";
import Card from "../components/CardComponent.vue";
import PriceCard from "../components/PriceCard.vue";
export default {
  components: { NavBar, Card, PriceCard },
};
</script>

<style scoped>
.home {
  width: 100vw;
  min-height: 100vh;
  background-color: black;
  padding-top: 125px;
}
section {
  position: relative;
  width: 100vw;
  min-height: 100vh;
  color: white;
  padding-right: 125px;
  padding-left: 125px;
}

/*          Intro Section          */

#IntroSection {
  background: url("../assets/featured_image-8.png");
  background-size: cover;
  background-position: center center;
  background-repeat: no-repeat;
}
.contentContainer {
  width: 100%;
  height: 100vh;
}
#IntroSection .contentContainer {
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  align-items: flex-start;
}
.TextBox {
  display: flex;
  flex-direction: column;
  width: 50%;
  height: 50%;
}

.TextBox h1 {
  font-size: 112px;
  margin-bottom: 20px;
}
.TextBox p {
  font-size: 40px;
  font-weight: lighter;
  line-height: 46px;
  margin-bottom: 30px;
}
#register-btn {
  width: 450px;
  height: 75px;
  border-radius: 5px;
  font-size: 30px;
  background-color: #f06130;
}

/*          Dance Tour Section          */

#DanceTour {
  padding-top: 125px;
  padding-bottom: 75px;
  text-align: center;
  background-image: repeating-linear-gradient(
      112.5deg,
      #f06130 0px,
      #f06130 20px,
      transparent 20px,
      transparent 22px
    ),
    repeating-linear-gradient(
      22.5deg,
      #f06130 0px,
      #f06130 20px,
      transparent 20px,
      transparent 22px
    ),
    linear-gradient(90deg, rgb(0, 0, 0), rgb(0, 0, 0));
}
#DanceTour .textContainer,
#Pricing .textContainer {
  margin: 0 auto;
  width: 70%;
  margin-bottom: 75px;
}
#DanceTour h1,
#Pricing h1 {
  font-size: 92px;
  font-weight: bold;
}
#DanceTour p,
#Pricing p {
  font-size: 40px;
  font-weight: lighter;
  margin: 25px 0;
}
#DanceTour .cardsContainer,
#Pricing .cardsContainer {
  width: 100%;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  column-gap: 80px;
}

/*          Pricing Section          */

#Pricing {
  padding-top: 125px;
  padding-bottom: 75px;
  text-align: center;
  background-image: repeating-linear-gradient(
      112.5deg,
      #2c2c2c 0px,
      #2c2c2c 20px,
      transparent 20px,
      transparent 22px
    ),
    repeating-linear-gradient(
      22.5deg,
      #2c2c2c 0px,
      #2c2c2c 20px,
      transparent 20px,
      transparent 22px
    ),
    linear-gradient(90deg, #4e4e4e, #4e4e4e);
}
</style>
