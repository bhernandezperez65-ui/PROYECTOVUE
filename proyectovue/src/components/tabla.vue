<template>
  <div>
    <h1>Comidas Típicas de El Salvador</h1>
    <table>
      <thead>
        <tr>
          <th>Comida</th>
          <th>Descripción</th>
          <th>Ingredientes Principales</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(comida, index) in comidas" :key="index">
          <td>{{ comida.nombre }}</td>
          <td>{{ comida.descripcion }}</td>
          <td>{{ comida.ingredientes.join(', ') }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  data() {
    return {
      comidas: [
        {
          nombre: 'Pupusas',
          descripcion: 'Tortillas rellenas típicas, muy populares.',
          ingredientes: ['Queso', 'Frijoles', 'Chicharrón', 'Maíz o arroz']
        },
        {
          nombre: 'Yuca frita o sancochada',
          descripcion: 'Servida con chicharrón y curtido.',
          ingredientes: ['Yuca', 'Chicharrón', 'Repollo', 'Zanahoria']
        },
        {
          nombre: 'Tamales',
          descripcion: 'Envueltos en hojas de plátano, típicos en celebraciones.',
          ingredientes: ['Maíz', 'Pollo o cerdo', 'Papas', 'Especias']
        },
        {
          nombre: 'Pan con pollo',
          descripcion: 'Pan relleno con pollo guisado y vegetales.',
          ingredientes: ['Pollo', 'Pan francés', 'Lechuga', 'Tomate', 'Pepino']
        },
        {
          nombre: 'Empanadas de plátano',
          descripcion: 'Postre tradicional relleno con frijol o leche.',
          ingredientes: ['Plátano maduro', 'Frijol dulce o leche', 'Azúcar']
        }
      ]
    };
  }
};
</script>

<style scoped>
table {
  width: 100%;
  border-collapse: collapse;
  margin-top: 20px;
}

th, td {
  padding: 12px;
  border: 1px solid #ddd;
  text-align: left;
}

th {
  background-color: #f8f8f8;
}
</style>
