<template>
  <div>
  <Componenteinicio></Componenteinicio>
  <tabla></tabla>
  </div>
</template>

<script>
import Componenteinicio from './components/componenteinicio.vue';
import HelloWorld from './components/HelloWorld.vue'
import tabla from './components/tabla.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
    Componenteinicio,
    Tabla
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
  margin-top: 60px;
}
</style>
