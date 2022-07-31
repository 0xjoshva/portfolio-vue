<template>
  <Home />
  <Featured/>
  <About />
  <Testimonial />
  <Footer/>
</template>

<script>
import Home from "../components/Home.vue";
import About from "../components/About.vue";
import Featured from "../components/Featured.vue";
import Testimonial from "../components/Testimonial.vue";
import Footer from "../components/Footer.vue";
export default {
  name: "HomeView",
  components: { Home, About, Featured, Footer, Testimonial },
};
</script>

<style></style>
