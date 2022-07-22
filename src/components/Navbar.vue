<template>
  <nav class="sticky-top">
    
    <div>
    <router-link to="/" id="logo"
      ><img src="../assets/newlogo.png" alt="logo" id="logo"
    /></router-link>
    </div>

    <div id="nav-links">
      <router-link to="/">HOME</router-link>
      <router-link to="/projects">PROJECTS</router-link>
      <router-link to="/contact">CONTACT</router-link>
    </div>
  </nav>
</template>
<script>
export default {};
</script>
<style scoped>
#logo {
  width: 130px;
  height: auto;
}
nav a {
  text-decoration: none;
  color: inherit;
}
nav {
  background: var(--bg-color);
  color: white;
  display: flex;
  justify-content: space-between;
  align-items: center;
  column-gap: 10px;
  font-family: "Montserrat", sans-serif;
  font-weight: 500;
  font-size: 13px;
  padding: 20px;
  border-bottom: 1px solid var(--dgrey);
  width: 100%;
}
#nav-links {
  display: flex;
  column-gap: 20px;
}
</style>
