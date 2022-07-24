<template>
  <Home />
  <Portfolio />
  <About />
  <Testimonial />
  <Footer />
</template>

<script>
import Home from "../components/Home.vue";
import About from "../components/About.vue";
import Portfolio from "../components/Portfolio.vue";
import Testimonial from "../components/Testimonial.vue";
import Footer from "../components/Footer.vue";
export default {
  name: "HomeView",
  components: { Home, About, Portfolio, Footer, Testimonial },
};
</script>

<style></style>
