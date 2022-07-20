<template>
  <Home />
  <About />
  <Portfolio />
  <Experience />
  <Footer />
</template>

<script>
import Home from "../components/Home.vue";
import Experience from "../components/Experience.vue";
import About from "../components/About.vue";
import Portfolio from "../components/Portfolio.vue";
import Footer from "../components/Footer.vue";
export default {
  name: "HomeView",
  components: { Home, About, Portfolio, Experience, Footer },
};
</script>

<style></style>
