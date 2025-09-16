<template>
  <nav class="navbar">
    <RouterLink to="/" class="logo">
     
    </RouterLink>
    <ul class="menu">
      <li v-for="item in menuItems" :key="item.name">
        <RouterLink :to="item.path">{{ item.name }}</RouterLink>
      </li>
    </ul>
  </nav>
</template>

<script setup>
const menuItems = [
  { name: "Inicio", path: "/" },
  { name: "Servicios", path: "/servicios" },
  { name: "Acerca", path: "/acerca" },
  { name: "Contacto", path: "/contacto" },
]
</script>

<style scoped>
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 15px 30px;
  background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);
  backdrop-filter: blur(10px);
  border-radius: 12px;
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
  position: sticky;
  top: 0;
  z-index: 1000;
}

.logo {
  display: flex;
  align-items: center;
  text-decoration: none;
}

.logo-img {
  height: 50px;
  width: auto;
  transition: transform 0.3s ease, filter 0.3s ease;
  filter: drop-shadow(0 2px 4px rgba(0, 0, 0, 0.3));
}

.logo-img:hover {
  transform: scale(1.05);
  filter: brightness(1.2) saturate(1.2);
}

.menu {
  list-style: none;
  display: flex;
  gap: 25px;
}

.menu li a {
  position: relative;
  text-decoration: none;
  color: white;
  font-weight: 500;
  font-size: 1rem;
  transition: color 0.3s ease;
}

.menu li a::after {
  content: "";
  position: absolute;
  left: 0;
  bottom: -4px;
  width: 0%;
  height: 2px;
  background-color: white;
  transition: width 0.3s ease;
}

.menu li a:hover::after {
  width: 100%;
}

.menu li a.router-link-exact-active {
  font-weight: 600;
  color: #ffe;
}

@media (max-width: 768px) {
  .navbar {
    flex-direction: column;
    align-items: flex-start;
    padding: 20px;
  }

  .menu {
    flex-direction: column;
    gap: 15px;
    margin-top: 10px;
  }
}
</style>
