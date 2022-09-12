<template>
  <div>
    <Navbar />
    <img class="banner-image" src="@/assets/banner-image.svg" />
    <p class="heading">Hot Game</p>
    <GameCard />
    <Information />

    <GameCategories />
    <Footer />
  </div>
</template>

<script>
import GameCard from "./components/GameCard.vue";
import Navbar from "./components/Navbar.vue";
import Information from "./components/Information.vue";
import Footer from "./components/Footer.vue";
import GameCategories from "./components/GameCategories.vue";
export default {
  name: "App",
  components: {
    GameCard,
    Navbar,
    Information,
    Footer,
    GameCategories,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* padding: 1rem; */
  background: #0f0f0f;
  height: 100%;
  width: 100%;
  /* overflow: hidden; */
}
p {
  margin: 0px;
}
ul {
  list-style: none;
  margin: 0px;
  padding: 0px;
}
.banner-image {
  width: 100%;
  height: 100px;
}
.heading {
  color: #c69a3a;
  margin: 1rem 0rem;
  padding: 0rem 1rem;
}
</style>
