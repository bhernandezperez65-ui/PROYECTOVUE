<template>
  <div>
    <p v-bind:class="classColor" :style="styles">Restaurante <br>
      Las Olivas</p>
    <img :src="imagen" v-bind:alt="texto">

  </div>
</template>

<script>
export default {
  name: 'Componenteinicio',
  data() {
    return {
      imagen:
        "https://i.pinimg.com/736x/6d/32/18/6d3218b9c7e28faefd766fa0b3d95713.jpg",

      texto: 'Logo Vue',
      classColor: 'text',
      styles: {
        'font-size': '30px',
        'font-weight': 'bold',
        'background-color': '#6A2C1D',
        'padding': '20px',
        'width': '300px',
        'display': 'block',
        'margin': '0 auto',
        'border-radius': '20px'
      }
    }

  }

}
</script>

<style>
img {
  height: 500px;
  width: 30%;
}

.text {
  color: #EC9843;
  text-align: center;
}
</style>