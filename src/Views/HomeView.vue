<template>
  <main class="home">
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

    <section class="Showcase" id="Showcase 1">
      <div class="ImageContainer"></div>
      <div class="textContainer">
        <h1>AMAZING DANCE</h1>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Corporis
          ullam sit ducimus ea eos ratione?
        </p>
        <button>READ MORE</button>
      </div>
    </section>

    <section class="Showcase" id="Showcase2">
      <div class="ImageContainer"></div>
      <div class="textContainer">
        <h1>DANCE BEST</h1>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Corporis
          ullam sit ducimus ea eos ratione?
        </p>
        <button>READ MORE</button>
      </div>
    </section>

    <section id="Statistics">
      <div class="contentContainer">
        <div class="textContainer">
          <h1>OUR STATISTICS</h1>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Corporis
            ullam sit ducimus ea eos ratione?
          </p>
        </div>
        <div class="cardsContainer">
          <StatComponent Title="Club" v-bind:Digit="1240"></StatComponent>
          <StatComponent
            Title="Active Member"
            v-bind:Digit="2000"
          ></StatComponent>
          <StatComponent Title="Community" v-bind:Digit="1000"></StatComponent>
        </div>
      </div>
    </section>

    <section id="Quote">
      <div class="textContainer">
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit
          eveniet at est perferendis accusamus.
        </p>
        <h1>HERBERT SIMON</h1>
      </div>
    </section>

    <section id="Subscription">
      <div class="contentContainer">
        <div class="textContainer">
          <h1>SUBSCRIBE</h1>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit
            eveniet at est perferendis accusamus.
          </p>
          <form action="">
            <input type="email" class="" placeholder="Your Email" />
            <input type="submit" value="SUBSCIRBE" />
          </form>
        </div>
      </div>
    </section>
    <footer>
      <div class="musicology">
        <h1>MUSICOLOGY</h1>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Amet
          pariatur aliquid eaque numquam magnam maxime quam eveniet. Cumque quia
          inventore deleniti!
        </p>
        <div class="iconContainer">
          <v-icon color="#2c2c2c">mdi-instagram</v-icon>
          <v-icon color="#2c2c2c">mdi-facebook</v-icon>
          <!-- <i class="fab fa-facebook-f"></i> -->
          <v-icon color="#2c2c2c">mdi-twitter</v-icon>
          <v-icon color="#2c2c2c">mdi-whatsapp</v-icon>
        </div>
      </div>
      <div class="sideContent">
        <div class="about">
          <h1>ABOUT</h1>
          <ul>
            <li>History</li>
            <li>Our Team</li>
            <li>Brand Guidelines</li>
            <li>Terms & Conditions</li>
            <li>Privacy policy</li>
          </ul>
        </div>
        <div class="services">
          <h1>SERVICES</h1>
          <ul>
            <li>How To Order</li>
            <li>Our Product</li>
            <li>Order Status</li>
            <li>Promo</li>
            <li>Payment Method</li>
          </ul>
        </div>
        <div class="other">
          <h1>OTHER</h1>
          <ul>
            <li>Contact Us</li>
            <li>Help</li>
            <li>Privacy</li>
          </ul>
        </div>
      </div>
    </footer>
  </main>
</template>
<script>
import NavBar from "../components/NavBar.vue";
import Card from "../components/CardComponent.vue";
import PriceCard from "../components/PriceCard.vue";
import StatComponent from "@/components/StatComponent.vue";
export default {
  components: { NavBar, Card, PriceCard, StatComponent },
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
  position: relative;
  bottom: 250px;
  display: flex;
  flex-direction: column;
  width: 50%;
}

.TextBox h1 {
  font-size: 142px;
  margin-bottom: 20px;
}
.TextBox p {
  font-size: 52px;
  font-weight: lighter;
  line-height: 52px;
  margin-bottom: 60px;
}
#register-btn {
  width: 400px;
  height: 80px;
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
#Pricing .textContainer,
#Statistics .textContainer,
#Quote .textContainer,
#Subscription .textContainer {
  text-align: center;
  margin: 0 auto;
  width: 70%;
  margin-bottom: 75px;
}
#DanceTour h1,
#Pricing h1,
.Showcase h1,
#Statistics h1,
#Subscription h1 {
  font-size: 92px;
  font-weight: bold;
}
#DanceTour p,
#Pricing p,
#Statistics p,
#Subscription p {
  font-size: 40px;
  font-weight: lighter;
  margin: 25px 0;
}
#DanceTour .cardsContainer,
#Pricing .cardsContainer,
#Statistics .cardsContainer {
  width: 100%;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  column-gap: 80px;
}

/*          Pricing Section          */

#Pricing {
  padding-top: 125px;
  padding-bottom: 175px;
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

/*          Showcase Section          */

.Showcase {
  padding: 0 !important;
  display: flex;
  background-image: repeating-linear-gradient(
      112.5deg,
      #ff6309 0px,
      #ff6309 20px,
      transparent 20px,
      transparent 22px
    ),
    repeating-linear-gradient(
      22.5deg,
      #ff6309 0px,
      #ff6309 20px,
      transparent 20px,
      transparent 22px
    ),
    linear-gradient(90deg, rgb(0, 0, 0), rgb(0, 0, 0));
}
.ImageContainer {
  width: calc(50vw - 2px);
  height: 100vh;
  background: url("../assets/21dc2fc3edd08e57fea63b977ea3f6ed.jpg");
  background-size: cover;
  background-position: center center;
  background-repeat: no-repeat;
}
.Showcase .textContainer {
  position: relative;
  top: 25px;
  padding-left: 125px;
  padding-right: 125px;
  width: 50%;
  height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: center;
}
.Showcase .textContainer p {
  font-size: 42px;
  font-weight: lighter;
  margin-bottom: 75px;
}
.Showcase button {
  padding: 12.5px 125px;
  font-size: 36px;
  background: #2c2c2c;
  border-radius: 5px;
}
#Showcase2 {
  flex-direction: row-reverse;
}

/*          Showcase Section          */

#Statistics {
  background-color: #2c2c2c;
  padding-top: 200px;
}
#Statistics .textContainer {
  margin-bottom: 175px;
}

/*          Quotes Section          */

#Quote {
  background: #ff6309;
  position: relative;
  background-image: url("../assets/featured_image-8.png");
  background-size: cover;
  background-position: center center;
  background-repeat: no-repeat;
  background-blend-mode: luminosity;
  display: flex;
  justify-content: center;
  align-items: center;
}
#Quote .textContainer {
  width: 100%;
  padding: 0 250px;
}

#Quote h1 {
  font-size: 80px;
  font-weight: bold;
}
#Quote p {
  font-size: 60px;
  margin-bottom: 75px;
}

/*          Subscription Section          */
#Subscription {
  background-color: #ff6309;
  min-height: fit-content !important;
}
#Subscription .contentContainer {
  padding-top: 125px;
  height: 730px;
}
#Subscription form {
  width: 100%;
  height: 100px;
  display: flex;
  align-items: center;
  justify-content: center;
}
#Subscription input[type="email"] {
  border: none;
  outline: none;
  padding-left: 50px;
  width: 700px;
  height: 75px;
  background: white;
}

#Subscription input[type="email"]::placeholder {
  color: grey;
  font-size: 40px;
  font-weight: 400;
}
#Subscription input[type="submit"] {
  width: 275px;
  font-size: 34px;
  height: 78px;
  background: #2c2c2c;
  border-top-right-radius: 5px;
  border-bottom-right-radius: 5px;
}
footer {
  padding: 140px 75px 150px 75px;
  width: 100vw;
  height: 600px;
  background: #2c2c2c;
  display: flex;
  justify-content: space-around;
  color: white;
}
footer h1 {
  font-size: 48px;
  margin-bottom: 25px;
}
footer p {
  font-size: 30px;
  margin-bottom: 50px;
}
footer ul {
  list-style: none;
  height: 100%;
  font-size: 38px;
}
footer .musicology,
footer .sideContent {
  width: 50%;
  height: 100%;
}
footer .musicology {
  padding-right: 250px;
}
footer .sideContent {
  width: 50%;
  height: 100%;
  display: flex;
  justify-content: space-between;
}
footer .iconContainer {
  width: 250px;
  height: 100px;
  display: flex;
  justify-content: space-between;
}
footer .iconContainer * {
  color: #2c2c2c;
  font-size: 36px;

  width: 50px;
  height: 50px;
  border-radius: 50%;
  background: white;
}
</style>
