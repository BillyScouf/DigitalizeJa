<!-- src/components/About.vue -->
<template>
  <section id="sobre" class="about">
    <div class="text">
      <h2>Sobre Nós</h2>
      <p>
        No DigitalizaJá, acreditamos que cada empresa, independentemente do tamanho, 
        merece estar presente no mundo digital de forma profissional e impactante. 
        Nossa missão é transformar ideias em sites estáticos modernos, responsivos e fáceis de usar, 
        que representem verdadeiramente a identidade de cada cliente. </p>

       <p>Combinamos criatividade, tecnologia e atenção aos detalhes para entregar soluções digitais 
        que não apenas impressionam visualmente, mas também facilitam a experiência do usuário. 
        Queremos que sua empresa seja vista, lembrada e valorizada na era digital — e fazemos isso de maneira rápida, 
        eficiente e acessível.
        </p>
        <p> No DigitalizaJá, sua presença online não é apenas um site, é o primeiro passo para novas oportunidades, clientes e crescimento.
      </p><br><br>

      <a class="cta" target="_blank" href="https://www.linkedin.com/in/and%C3%A9rsiolopes/" >Meu LinkedIn</a>
    </div>

    <div class="image"></div>
  </section>
</template>

<style scoped>
.about {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 4rem 2rem;
  background: #0f172a;
  color: white;
  gap: 2rem;
}

.text {
  max-width: 50%;
}

.image {
  width: 480px;
  height: 360px;
  border-radius: 12px;
  /* background: radial-gradient(circle, #60a5fa 20%, #1e3a8a 80%); */
  background-image: url("../../public/img/how-to-start-web-design-business.jpeg");
  background-repeat: no-repeat;
  background-position: top center;
}

.cta {
  margin-top: 2rem;
  background: rgb(255, 255, 255);
  color: black;
  padding: 0.8rem 1.8rem;
  border-radius: 8px;
  border: none;
  cursor: pointer;
  text-decoration: none;
  display: inline-block;
}

.cta:hover {
  background: #2563eb;
  transition: all 0.3s;
  color: #fff;
}

/* RESPONSIVO */
@media (max-width: 1024px) {
  .about {
    flex-direction: column;
    align-items: center;
    text-align: center;
    gap: 2rem;
  }
  .text {
    max-width: 90%;
  }
  .image {
    width: 300px;
    height: 200px;
  }
}

@media (max-width: 480px) {
  .about {
    padding: 2rem 1rem;
    gap: 1.5rem;
  }
  .text h2 {
    font-size: 1.5rem;
  }
  .text p {
    font-size: 0.95rem;
  }
  .image {
    width: 100%;
    max-width: 250px;
    height: 160px;
  }
  .cta {
    padding: 0.6rem 1.2rem;
    font-size: 0.9rem;
  }
}
</style>
