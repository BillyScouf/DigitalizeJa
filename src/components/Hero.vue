<!-- src/components/Hero.vue -->
<template>
  <section id="home" class="hero">
    <h1>Criação de sites profissionais para pequenas e médias empresas</h1>
    <p>Transformando desafios em resultados digitais.</p>

    <button class="cta">Contacte-me</button>
  </section>
</template>

<style scoped>
.hero {
  text-align: center;
  padding: 5rem 2rem;
  background: #ffffff;
}

h1 {
  font-size: 2.5rem;
  max-width: 700px;
  margin: auto;
  font-weight: 800;
}

p {
  margin-top: 1rem;
  color: #555;
}

.cta {
  margin-top: 2rem;
  background: black;
  color: white;
  padding: 0.8rem 1.8rem;
  border-radius: 8px;
  border: none;
  cursor: pointer;
}
.cta:hover {
  background: #2563eb;
  transition: all .3s ;
}
</style>
