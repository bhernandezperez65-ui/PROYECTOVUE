<template>
  <div class="comida">
    <h1>🍽️ Menú de Restaurante</h1>

    <h2>Platillos disponibles</h2>
    <ul>
      <li v-for="(platillo, index) in platillos" :key="index">🍴 {{ platillo }}</li>
    </ul>

    <h2>Selecciona tu favorito</h2>
    <select v-model="seleccionado">
      <option disabled value="">-- Elige uno --</option>
      <option v-for="(platillo, index) in platillos" :key="index" :value="platillo">
        {{ platillo }}
      </option>
    </select>

    <div v-if="seleccionado" class="resultado">
      <p>✨ Elegiste: <strong>{{ seleccionado }}</strong></p>
    </div>
  </div>
</template>

<script>
export default {
  name: "MenuRestaurante",
  data() {
    return {
      platillos: [
        'Pollo en salsa de hongos',
        'Sopa de tomate con albahaca',
        'Pasta con salsa Alfredo',
        'Ensalada César con pollo',
        'Filete de pescado empanizado',
        'Hamburguesa con queso y papas',
        'Lasaña de carne',
        'Nuggets de pollo con papas fritas',
        'Pollo a la plancha con vegetales',
        'Pasta boloñesa',
        'Crema de brócoli',
        'Tacos de carne con guacamole',
        'Sandwich club con papas',
        'Pizza de pepperoni',
        'Omelette de jamón y queso',
        'Quesadillas de pollo',
        'Arroz con pollo',
        'Sopa de lentejas',
        'Pollo BBQ con ensalada',
        'Croquetas de papa con queso'
      ],
      seleccionado: ''
    }
  }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;700&display=swap');

.comida {
  background: linear-gradient(135deg, #e1f5fe, #f3e5f5);
  padding: 30px;
  border-radius: 18px;
  font-family: 'Poppins', sans-serif;
  color: #3e2723;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}

h1 {
  text-align: center;
  font-size: 30px;
  margin-bottom: 20px;
  font-weight: 700;
  color: #6a1b9a;
}

h2 {
  font-size: 20px;
  margin-top: 25px;
  font-weight: 600;
  color: #4a148c;
}

ul {
  list-style-type: none;
  padding-left: 0;
  columns: 2;
}

li {
  margin-bottom: 8px;
  font-size: 16px;
  background-color: rgba(255,255,255,0.6);
  padding: 6px 10px;
  border-radius: 6px;
}

select {
  margin-top: 15px;
  padding: 10px;
  border-radius: 8px;
  border: 1px solid #ce93d8;
  background-color: #fff;
  color: #6a1b9a;
  font-family: 'Poppins', sans-serif;
  font-size: 16px;
  width: 100%;
  max-width: 320px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.1);
}

.resultado {
  margin-top: 25px;
  background-color: rgba(255, 255, 255, 0.85);
  padding: 14px;
  border-left: 5px solid #ba68c8;
  font-size: 18px;
  font-weight: 600;
  color: #4e342e;
  border-radius: 8px;
}
</style>
