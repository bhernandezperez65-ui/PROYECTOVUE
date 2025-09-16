<template>
  <div>
  <Navbar></Navbar>
  <Componenteinicio></Componenteinicio>
  </div>
</template>

<script>
import Componenteinicio from './components/componenteinicio.vue';
import HelloWorld from './components/HelloWorld.vue'
import Navbar from './components/Navbar.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
    Componenteinicio,
    Navbar
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
