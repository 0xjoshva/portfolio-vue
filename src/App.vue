<template>
  <Navbar />
  <router-view />
</template>
<script>
import Navbar from "./components/Navbar.vue";
export default {
  name: "App",
  components: { Navbar },
  // return: { dark : true},
  //   methods = {
  //     let root = document.querySelector(":root"),
  //     if(dark) {
  //       root.style.setProperty('--bg-color', '#YOURCOLOR'),
  //       root.style.setProperty('--dgrey', '#YOURCOLOR'),
  //       root.style.setProperty('--lgrey', '#YOURCOLOR'),
  //       root.style.setProperty('--white', '#YOURCOLOR'),
  //       root.style.setProperty('--green', '#YOURCOLOR'),
  //       root.style.setProperty('--lgreen', '#YOURCOLOR'),
  //     }
  //     else {
  //       root.style.setProperty('--bg-color', '#YOURCOLOR'),
  //       root.style.setProperty('--dgrey', '#YOURCOLOR'),
  //       root.style.setProperty('--lgrey', '#YOURCOLOR'),
  //       root.style.setProperty('--white', '#YOURCOLOR'),
  //       root.style.setProperty('--green', '#YOURCOLOR'),
  //       root.style.setProperty('--lgreen', '#YOURCOLOR'),
  //     }
  //   }
};
</script>
<style>
@import url("https://cdn.jsdelivr.net/npm/bootstrap-icons@1.9.1/font/bootstrap-icons.css");
/* FONTS */
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@100;300;500;700;900&family=Palanquin:wght@200;400;600;700&family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap");
/* font-family: 'Montserrat', sans-serif;
font-family: 'Palanquin', sans-serif;
font-family: 'Roboto', sans-serif; */
/* CSS RESET */
html {
  box-sizing: border-box;
  font-size: 16px;
  scroll-behavior: smooth;
}

*,
*:before,
*:after {
  box-sizing: inherit;
}

body,
h1,
h2,
h3,
h4,
h5,
h6,
p,
ol,
ul {
  margin: 0;
  padding: 0;
  font-weight: normal;
}

ol,
ul {
  list-style: none;
}

img {
  max-width: 100%;
  height: auto;
}

/* COLOR SCHEME */
:root {
  /* backgrounds */
  --bg-color: #101010;
  --dgrey: #1d1d1d;
  /* highlights */
  --green: #1db954;
  --lgreen: #00e472;
  /* for text */
  --lgrey: #8f8f8f;
  --white: #f1f1f1;
}

::-webkit-scrollbar-track {
  -webkit-box-shadow: inset 0 0 6px var(--bg-color);
  box-shadow: inset 0 0 6px var(--bg-color);
  border-radius: 10px;
  background-color: var(--bg-color);
}

::-webkit-scrollbar {
  width: 12px;
  background-color: var(--bg-color);
}

::-webkit-scrollbar-thumb {
  border-radius: 10px;
  -webkit-box-shadow: inset 0 0 6px rgba(0, 0, 0, 0.3);
  box-shadow: inset 0 0 6px rgba(0, 0, 0, 0.3);
  background-color: var(--lgrey);
}

nav a :active {
  color: var(--lgreen);
}
</style>
