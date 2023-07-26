<script setup>
</script>
<template>
  <footer class="footer push">
    <div class="container">
      <div class="footer_row">
        <div class="footer_links">
          <h4>DEVKAREN</h4>
          <ul>
            <li><a href="#">Nosotros</a></li>
            <li><a href="#">Nuestros servicios</a></li>
            <li><a href="#">Policitica de privacidad</a></li>
            <li><a href="#">Afiliate</a></li>
          </ul>
        </div>
        <div class="footer_links">
          <h4>Contáctame</h4>
          <div class="social_link">
            <a
              href="https://www.linkedin.com/in/karen-yulier-rodriguez/"
              target="_blank"
              ><i class="fab fa-linkedin"></i
            ></a>
            <a href="https://github.com/karenyulierr" target="_blank"
              ><i class="fab fa-github"></i
            ></a>
            <a
              href="https://api.whatsapp.com/send?phone=573143960806"
              target="_blank"
            >
              <i class="fab fa-whatsapp"></i>
            </a>
            <a href="mailto:karenyulierr@gmail.com" target="_blank">
              <i class="fa-solid fa-at"></i>
            </a>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<style scoped>
.push {
  flex: 1;
}
.container {
  max-width: 1200px;
  margin: 0 auto;
}
.footer {
  background-color: var(--azul_oscuro);
  padding: 80px 0;
}
.footer_row {
  display: flex;
  flex-wrap: wrap;
}
.footer_links {
  width: 50%;
  padding: 0 15px;
}
.footer_links h4 {
  font-size: 20px;
  color: var(--blanco);
  margin-bottom: 25px;
  font-weight: 500;
  border-bottom: 2px solid var(--blanco);
  padding-bottom: 10px;
  display: inline-block;
}
.footer_links ul {
  list-style: none;
}
.footer_links ul li a {
  font-size: 18px;
  text-decoration: none;
  color: var(--blanco);
  display: block;
  margin-bottom: 15px;
  transition: all 0.3s ease;
}
.footer_links ul li a:hover {
  color: var(--azul_claro);
  padding-left: 6px;
}
.footer_links ul {
  margin: 0;
  padding: 0;
}
.social_link a {
  display: inline-block;
  min-height: 40px;
  width: 40px;
  background-color: rgba(255, 255, 255, 0.2);
  margin: 0 10px 10px 0;
  text-align: center;
  line-height: 40px;
  border-radius: 50%;
  color: var(--blanco);
  transition: all 0.5s ease;
}
.social_link a:hover {
  background-color: var(--azul_oscuro);
}

@media (max-width: 991px) {
  .footer_row {
    text-align: center;
  }
  .footer_links {
    width: 100%;
    margin-bottom: 30px;
  }
}
</style>