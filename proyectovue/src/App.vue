<template>
  <div>
  <Navbar></Navbar>
  <Componenteinicio></Componenteinicio>
  <tabla></tabla>
  <list></list>
  <comida></comida>
  <footer></footer>
  </div>
</template>

<script>
import Componenteinicio from './components/componenteinicio.vue';
import HelloWorld from './components/HelloWorld.vue'
import tabla from './components/tabla.vue';
import list from './components/list.vue';
import Navbar from './components/Navbar.vue';
import Comida from './components/Comida.vue';
import footer from './components/footer.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
    Componenteinicio,
    tabla,
    list,
    Navbar,
    Comida,
    footer
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
