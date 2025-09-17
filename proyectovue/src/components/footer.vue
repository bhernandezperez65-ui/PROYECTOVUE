<template>
  <footer class="footer">
    <div class="footer-content">
      <h3>🍽️ ProyectoWeb - Restaurante Los Olivos</h3>
      <p>
        Explorando la riqueza culinaria salvadoreña con pasión y sabor.  
      </p>
      <nav class="footer-links">
        <a href="#">Inicio</a>
        <a href="#">Recetas</a>
        <a href="#">Nutrición</a>
        <a href="#">Contacto</a>
      </nav>
      <small>© 2025 ProyectoWeb. Todos los derechos reservados.</small>
    </div>
  </footer>
</template>

<style scoped>
.footer {
  background-color: #fff8f2; /* fondo crema suave */
  border-top: 2px solid #e6cfc2; /* línea tostada clara */
  padding: 30px 0;
  text-align: center;
  font-family: 'Segoe UI', sans-serif;
  color: #5a3e36; /* texto marrón cálido */
}

.footer-content h3 {
  font-size: 1.4rem;
  margin-bottom: 10px;
  color: #a0522d; /* terracota */
}

.footer-content p {
  font-size: 0.95rem;
  margin-bottom: 20px;
  color: #6b4c3b;
}

.footer-links {
  margin-bottom: 20px;
}

.footer-links a {
  margin: 0 10px;
  color: #d96c4a; /* acento rojizo suave */
  text-decoration: none;
  font-weight: 500;
  transition: color 0.3s ease;
}

.footer-links a:hover {
  color: #b94e2e; /* tono más intenso al pasar el mouse */
}

small {
  font-size: 0.85rem;
  color: #8c6e5f;
}
</style>
