<!-- src/components/Navbar.vue -->
<template>
  <nav class="navbar">
    <div class="logo"><a href="#home">DigitalizeJá</a></div>

    <!-- Botão Hamburger para mobile -->
    <div class="hamburger" @click="toggleMenu">
      <span></span>
      <span></span>
      <span></span>
    </div>

    <ul :class="['menu', { 'active': menuActive }]">
      <li><a href="#home">Página Inicial</a></li>
      <li><a href="#sobre">Sobre Mim</a></li>
      <li><a href="#servicos">Serviços</a></li>
    </ul>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      menuActive: false
    }
  },
  methods: {
    toggleMenu() {
      this.menuActive = !this.menuActive;
    }
  }
}
</script>

<style scoped>
.logo a {
  font-family: 'Playpen Sans', cursive;
  font-size: 1.5rem;
  font-weight: 700;
  color: #000;
}

.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2rem;
  background: #ffffff;
  color: #000;
  font-weight: bold;
  position: relative;
}

.menu {
  list-style: none;
  display: flex;
  gap: 2rem;
}

.menu a {
  color: #000;
  text-decoration: none;
  transition: color 0.3s;
}

.menu a:hover {
  color: #2563eb;
}

/* Hamburger menu - hidden em telas grandes */
.hamburger {
  display: none;
  flex-direction: column;
  gap: 5px;
  cursor: pointer;
}

.hamburger span {
  width: 25px;
  height: 3px;
  background: #1d1d1d;
  border-radius: 2px;
}

/* RESPONSIVO */
@media (max-width: 768px) {
  .menu {
    position: absolute;
    top: 100%;
    right: 30px;
    background: #ffffff;
    flex-direction: column;
    width: 200px;
    padding: 1rem;
    gap: 1rem;
    box-shadow: 0 8px 16px rgba(46, 46, 46, 0.2);
    opacity: 0;
    pointer-events: none;
    transform: translateY(-20px);
    transition: all 0.3s ease;
  }

  .menu.active {
    opacity: 1;
    pointer-events: auto;
    transform: translateY(0);
  }

  .hamburger {
    display: flex;
  }
}
</style>
