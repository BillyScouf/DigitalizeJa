<!-- src/App.vue -->
<template>
  <NavBar />
  <Hero />
  <About />
  <services />
  <Footer />
</template>

<script>
import NavBar from './components/NavBar.vue'
import Hero from './components/Hero.vue'
import About from './components/About.vue'
import services from './components/services.vue'
import Footer from './components/Footer.vue'

export default {
  components: { NavBar, Hero, About , services, Footer }
}
</script>

<style>

@import url('https://fonts.googleapis.com/css2?family=Playpen+Sans:wght@300;400;500;600;700&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');

body {
  font-family: 'Poppins', sans-serif;
  margin: 0;
}

*{
  box-sizing: border-box;
  text-decoration: none ;
}

</style>
