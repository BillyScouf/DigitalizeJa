<!-- src/components/Footer.vue -->
<template>
  <footer class="footer">
    <div class="left">
      <div class="logo"><a href="#home">DigitalizaJá</a></div>
      <p>Consultoria especializada em criação de sites estáticos modernos, rápidos e profissionais.</p>
    </div>

    <div class="grid">
      <div>
        <h4>Serviços</h4>
        <p>Sites Estáticos</p>
        <p>Landing Pages</p>
        <p>Portfólios</p>
        <p>Redesign de Sites</p>
      </div>

      <div>
        <h4>Recursos</h4>
        <p>Perguntas Frequentes</p>
        <p>Processo de Trabalho</p>
        <p>Exemplos de Sites</p>
      </div>

      <div>
        <h4>Contacto</h4>
        <p><a href="contacto.html">Página de Contacto</a></p>
        <p><a href="redes.html">Minhas Redes Sociais</a></p>
      </div>
    </div>

    <div class="footer-bottom">
      <p>&copy; 2025 DigitalizeJá. Todos os direitos reservados.</p>
    </div>

  </footer>
</template>

<style>
.footer {
  background-color: #111;
  color: #fff;
  padding: 50px 20px;
  font-family: 'Poppins', sans-serif;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 40px;
}

.footer .left {
  text-align: center;
}

.footer .left .logo a {
  color: #ffffff;
  font-weight: bold;
  font-size: 1.6rem;
  text-decoration: none;
}

.footer .left p {
  color: #ccc;
  max-width: 500px;
  margin: 10px auto 0;
}

.footer .grid {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
  gap: 30px;
  text-align: center;
  width: 100%;
  max-width: 1000px;
}

.footer .grid div h4 {
  margin-bottom: 15px;
  font-size: 1.2rem;
  color: #fff;
}

.footer .grid div p,
.footer .grid div a {
  margin: 5px 0;
  color: #ccc;
  text-decoration: none;
  transition: color 0.3s;
}

.footer .grid div p:hover,
.footer .grid div a:hover {
  color: #757575;
}

.footer .grid div a {
  display: inline-block;
}

.footer-bottom {
  text-align: center;
  font-size: 0.9rem;
  color: #000000;
  width: 100%;
  background-color: #fff;
}

/* RESPONSIVO */
@media (max-width: 768px) {
  .footer .grid {
    flex-direction: column;
    align-items: center;
    gap: 20px;
  }
  .footer .grid div {
    width: 80%;
  }
}

@media (max-width: 480px) {
  .footer .left p {
    font-size: 0.9rem;
  }
  .footer .grid div h4 {
    font-size: 1rem;
  }
  .footer .grid div p,
  .footer .grid div a {
    font-size: 0.9rem;
  }
}

</style>