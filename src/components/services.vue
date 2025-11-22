<!-- src/components/Services.vue -->

<script setup>
  import Swal from 'sweetalert2'

  function detalhesLandingPage() {
    Swal.fire({
      title: 'Landing Pages Profissionais',
      html: `
        <p style="text-align:left;">
          ✔️ Design moderno e responsivo<br>
          ✔️ Alta conversão<br>
          ✔️ Velocidade otimizada<br>
          ✔️ Hospedagem gratuita (Opcional)<br><br>

          <strong>Ideal para:</strong><br>
          - Serviços<br>
          - Campanhas<br>
          - Produtos<br>
          - Cartões de apresentação Digitail<br><br>

          <strong style="font-size:18px;">Preço: A partir de <span style="color:#0d6efd;"> ------- KZ</span></strong>
        </p>
      `,
      icon: 'info',
      confirmButtonText: 'Fechar',
      confirmButtonColor: '#0d6efd',
      width: '450px'
    })
}


// sweet do primeiro botao

function mostrarAlerta() {
  Swal.fire({
    title: 'Criação de Sites Estáticos',
    html: `
      <p style="text-align:left;">
        Sites estáticos rápidos, modernos e otimizados para negócios que precisam de presença digital sólida e profissional.<br><br>

        <strong>Inclui:</strong><br>
        ✔️ Layout moderno e responsivo<br>
        ✔️ Até 5 secções (Home, Sobre, Serviços, Contactos, etc.)<br>
        ✔️ SEO básico<br>
        ✔️ Hospedagem gratuita<br><br>

        <strong style="font-size:18px;">Preço: A partir de <span style="color:#0d6efd;"> ------- KZ</span></strong>
      </p>
    `,
    icon: 'info',
    width: '480px',
    confirmButtonText: 'Fechar',
    confirmButtonColor: '#0d6efd'
  })
}

// portofolio
function mostrarPortfolio() {
  Swal.fire({
    title: 'Portfólios Pessoais',
    html: `
      <p style="text-align:left;">
        Crie um portfólio moderno, elegante e totalmente responsivo para apresentar sua experiência, projetos e serviços de forma profissional.<br><br>

        <strong>Inclui:</strong><br>
        ✔️ Página personalizada com design elegante<br>
        ✔️ Secções: Sobre, Projetos, Skills, Contactos<br>
        ✔️ Galeria de projetos otimizada<br>
        ✔️ Hospedagem gratuita<br><br>

        <strong style="font-size:18px;">Preço: A partir de <span style="color:#0d6efd;"> ------- KZ</span></strong>
      </p>
    `,
    icon: 'info',
    width: '480px',
    confirmButtonText: 'Fechar',
    confirmButtonColor: '#0d6efd'
  })
}

// redesign
function mostrarRedesign() {
  Swal.fire({
    title: 'Redesign de Sites',
    html: `
      <p style="text-align:left;">
        Transformo sites antigos em versões modernas, rápidas e compatíveis com todos os dispositivos. O objetivo é melhorar o design, a experiência do usuário e o desempenho do site sem perder sua identidade.<br><br>

        <strong>Inclui:</strong><br>
        ✔️ Novo layout moderno e profissional<br>
        ✔️ Responsividade completa (mobile + tablet + desktop)<br>
        ✔️ Melhorias de velocidade e SEO<br>

        <strong style="font-size:18px;">
          Preço: A partir de <span style="color:#0d6efd;"> ------- KZ</span>
        </strong>
      </p>
    `,
    icon: 'info',
    width: '480px',
    confirmButtonText: 'Fechar',
    confirmButtonColor: '#0d6efd'
  })
}

// Hospedagem

function mostrarDeploy() {
  Swal.fire({
    title: 'Publicação & Deploy',
    html: `
      <p style="text-align:left;">
        Oferecemos hospedagem gratuita e deploy completo do seu site em plataformas confiáveis como Netlify, GitHub Pages, Render ou Vercel. Garantimos que seu site fique online rapidamente e sem complicações.<br><br>

        <strong>Inclui:</strong><br>
        ✔️ Configuração de domínio e subdomínio<br>
        ✔️ Deploy automático via GitHub<br>
        ✔️ Sites rápidos e seguros<br>
        ✔️ Monitoramento básico de uptime<br>
        ✔️ Suporte inicial após publicação<br><br>

        <strong style="font-size:18px;">
          Preço: Incluso nos pacotes digitais ou a partir de <span style="color:#0d6efd;"> ------- KZ</span>
        </strong>
      </p>
    `,
    icon: 'info',
    width: '480px',
    confirmButtonText: 'Fechar',
    confirmButtonColor: '#0d6efd'
  })
}
</script>

<template>
<section id="servicos" class="services">

  <div class="card">
    <h3>Criação de Sites Estáticos</h3>
    <p>Desenvolvimento de sites rápidos, modernos e totalmente responsivos para pequenas e médias empresas.</p>
    <button @click="mostrarAlerta()">Saiba mais → </button>
  </div>

  <div class="card">
    <h3>Landing Pages Profissionais</h3>
    <p>Páginas únicas focadas em conversão, ideais para campanhas, serviços e divulgação de produtos.</p>
    <button @click="detalhesLandingPage()">Saiba mais →</button>
  </div>

  <div class="card">
    <h3>Portfólios Pessoais</h3>
    <p>Mostre seus projetos e experiência com um portfólio elegante, simples e fácil de navegar.</p>
    <button @click="mostrarPortfolio()">Saiba mais →</button>
  </div>

  <div class="card">
    <h3>Redesign de Sites</h3>
    <p>Transformo sites antigos em versões modernas, leves e compatíveis com todos os dispositivos.</p>
    <button @click="mostrarRedesign()">Saiba mais →</button>
  </div>

  <div class="card">
    <h3>Publicação & Deploy</h3>
    <p>Hospedagem gratuita em Netlify, GitHub Pages, Render ou Vercel, com deploy completo.</p>
    <button @click="mostrarDeploy()">Saiba mais →</button>
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

.price {
  font-weight: bold;
  color: #ff6600; /* cor chamativa */
  margin-top: 10px;
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
.card button{
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
.card button:hover {
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
