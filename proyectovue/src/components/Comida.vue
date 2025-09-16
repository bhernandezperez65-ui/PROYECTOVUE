<template>
  <div class="contenedor">
    <h2>Comidas famosas del mundo</h2>

    <table class="tabla">
      <thead>
        <tr>
          <th>Código</th>
          <th>Platillo</th>
          <th>País de Origen</th>
          <th>Precio (USD)</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="comida in comidas" :key="comida.code">
          <td>{{ comida.code }}</td>
          <td>{{ comida.nombre }}</td>
          <td>{{ comida.pais }}</td>
          <td>{{ comida.precio }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  name: "Comidas",
  data() {
    return {
      comidas: [
        { code: 1, nombre: "Pizza", pais: "Italia", precio: 12 },
        { code: 2, nombre: "Sushi", pais: "Japón", precio: 18 },
        { code: 3, nombre: "Tacos", pais: "México", precio: 8 },
        { code: 4, nombre: "Curry", pais: "India", precio: 10 },
        { code: 5, nombre: "Pupusas", pais: "El Salvador", precio: 5 },
        { code: 6, nombre: "Croissant", pais: "Francia", precio: 4 },
        { code: 7, nombre: "Paella", pais: "España", precio: 20 },
        { code: 8, nombre: "Hot Dog", pais: "Estados Unidos", precio: 6 },
        { code: 9, nombre: "Feijoada", pais: "Brasil", precio: 14 },
        { code: 10, nombre: "Shawarma", pais: "Líbano", precio: 9 }
      ]
    };
  }
};
</script>

<style scoped>
.contenedor {
  text-align: center;
  padding: 20px;
  font-family: Arial, sans-serif;
}
.tabla {
  width: 70%;
  margin: 0 auto;
  border-collapse: collapse;
}
.tabla th {
  background: #f0f0f0;
  padding: 10px;
  border: 1px solid #ccc;
}
.tabla td {
  padding: 8px;
  border: 1px solid #ccc;
  text-align: center;
}
</style>
