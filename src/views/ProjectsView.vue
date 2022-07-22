<template>
  <Projects/>
  <Experience />
  <Footer />
</template>
<script>
import Experience from "../components/Experience.vue";
import Footer from "../components/Footer.vue";
import Projects from "../components/Projects.vue";
export default {
  components: { Footer, Experience, Projects },
};
</script>

<style>
</style>
