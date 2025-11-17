<!-- src/components/Services.vue -->
<template>
<section id="servicos" class="services">
  <div class="card">
    <h3>Criação de Sites Estáticos</h3>
    <p>Desenvolvimento de sites rápidos, modernos e totalmente responsivos para pequenas e médias empresas.</p>
    <a href="#">Saiba mais →</a>
  </div>

  <div class="card">
    <h3>Landing Pages Profissionais</h3>
    <p>Páginas únicas focadas em conversão, ideais para campanhas, serviços e divulgação de produtos.</p>
    <a href="#">Ver detalhes →</a>
  </div>

  <div class="card">
    <h3>Portfólios Pessoais</h3>
    <p>Mostre seus projetos e experiência com um portfólio elegante, simples e fácil de navegar.</p>
    <a href="#">Criar portfólio →</a>
  </div>

  <div class="card">
    <h3>Redesign de Sites</h3>
    <p>Transformo sites antigos em versões modernas, leves e compatíveis com todos os dispositivos.</p>
    <a href="#">Atualizar site →</a>
  </div>

  <div class="card">
    <h3>Publicação & Deploy</h3>
    <p>Hospedagem gratuita em Netlify, GitHub Pages, Render ou Vercel, com deploy completo.</p>
    <a href="#">Publicar site →</a>
  </div>
</section>

</template>

<style scoped>
/* Container da secção */
.services {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 1.5rem;
  padding: 2rem;
  max-width: 1100px;
  margin: auto;
}

/* Card */
.card {
  background: #ffffff;
  padding: 1.8rem;
  border-radius: 14px;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.08);
  transition: all 0.3s ease;
  border: 1px solid #f0f0f0;
}

/* Hover do card */
.card:hover {
  transform: translateY(-6px);
  box-shadow: 0 6px 26px rgba(0, 0, 0, 0.12);
}

/* Título */
.card h3 {
  font-size: 1.3rem;
  margin-bottom: 0.8rem;
  color: #222;
}

/* Texto */
.card p {
  font-size: 0.95rem;
  line-height: 1.5;
  margin-bottom: 1.2rem;
  color: #555;
}

/* Botão */
.card a {
  padding: 0.6rem 1.2rem;
  background: #007bff;
  color: white;
  border: none;
  border-radius: 8px;
  font-size: 0.95rem;
  cursor: pointer;
  transition: 0.3s ease;
}

/* Hover do botão */
.card a:hover {
  background: #005ec4;
}

/* Responsivo para ecrãs pequenos */
@media (max-width: 480px) {
  .card {
    padding: 1.5rem;
  }

  .card h3 {
    font-size: 1.15rem;
  }

  .card p {
    font-size: 0.9rem;
  }
}

</style>
