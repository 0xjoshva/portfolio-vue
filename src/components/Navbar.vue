<template>
    <nav>
    <router-link to="/">HOME</router-link>
    <router-link to="/portfolio">FOLIO</router-link>
    <router-link to="/contact">CONTACT</router-link>
  </nav>
</template>
<script>
export default {
    
}
</script>
<style scoped>

nav a{
  text-decoration: none;
  color: inherit;
}
    nav{
      background: var(--bg-color);
      color: white;
      display: flex;
      justify-content: flex-end;
      align-items: center;
      column-gap: 10px;
      font-family: 'Roboto', sans-serif;
      font-weight: 100;
      font-size: 13px;
      padding: 20px;
      border-bottom: 1px solid var(--dgrey);
    }

</style>