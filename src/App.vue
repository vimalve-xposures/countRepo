<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <div id="layout">
    <header> 
    <div class="wrapper">
      <nav>
        <RouterLink to="/">Home</RouterLink> |
        <RouterLink to="/about">About</RouterLink> |
        <RouterLink to="/count">Count</RouterLink>  |
        <RouterLink to="/singlecount">SingleCount</RouterLink> 
      </nav>
    </div>
  </header>

  <RouterView />
  </div>
</template>

<style scoped>
#layout{
  font-family: Avenir,Arial, Helvetica, sans-serif;
  -webkit-font-smoothening:antialiased;
  -moz-osx-font-smoothening:grayscale;
  text-align: center;
  color: #2c3e50;
}
nav{
  padding: 30px;
}
nav a{
  font-weight: bold;
  color: #2c3e50;
}
nav a.router-link-exact-active{
  color: #42b983;
}
</style>
