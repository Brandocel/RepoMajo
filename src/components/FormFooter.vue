<template>
  <footer class="footer">
    <div class="container">
      <div class="footer-content">
        <div class="footer-section about">
          <h2 class="logo-text">MiSitio</h2>
          <p>
            Este es un sitio web increíble construido con Vue.js.
          </p>
          <div class="contact">
            <span><i class="fas fa-phone"></i> &nbsp; +123-456-789</span>
            <span><i class="fas fa-envelope"></i> &nbsp; info@misitio.com</span>
          </div>
          <div class="socials">
            <a href="#"><i class="fab fa-facebook"></i></a>
            <a href="#"><i class="fab fa-twitter"></i></a>
            <a href="#"><i class="fab fa-instagram"></i></a>
            <a href="#"><i class="fab fa-linkedin"></i></a>
          </div>
        </div>

        <div class="footer-section links">
          <h2>Enlaces rápidos</h2>
          <br>
          <ul>
            <li><a href="#">Inicio</a></li>
            <li><a href="#">Sobre nosotros</a></li>
            <li><a href="#">Servicios</a></li>
            <li><a href="#">Contacto</a></li>
          </ul>
        </div>

        <div class="footer-section contact-form">
          <h2>Contáctanos</h2>
          <br>
          <form action="#" method="post">
            <input type="email" name="email" class="text-input contact-input" placeholder="Tu email...">
            <textarea name="message" class="text-input contact-input" placeholder="Tu mensaje..."></textarea>
            <button type="submit" class="btn btn-big">
              <i class="fas fa-envelope"></i>
              Enviar
            </button>
          </form>
        </div>
      </div>

      <div class="footer-bottom">
        &copy; misitio.com | Diseñado por Yo
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'AppFooter',
};
</script>

<style scoped>
.footer {
  background: linear-gradient(135deg, #3a3a3a, #1a1a1a);
  color: #fff;
  padding: 30px 0;
  text-align: center;
  transition: background 0.5s;
}

.footer:hover {
  background: linear-gradient(135deg, #4a4a4a, #2a2a2a);
}

.footer .container {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  flex-wrap: wrap;
  animation: fadeIn 1s ease-in-out;
}

.footer .footer-content {
  display: flex;
  justify-content: space-between;
  width: 100%;
}

.footer-section {
  flex: 1;
  padding: 20px;
  min-width: 250px;
}

.footer-section .logo-text {
  font-size: 1.8em;
  font-weight: 600;
  color: #ff3a6d;
  transition: color 0.5s;
}

.footer-section .logo-text:hover {
  color: #fff;
}

.footer-section .contact span,
.footer-section .socials a {
  display: block;
  margin-bottom: 10px;
  transition: transform 0.3s;
}

.footer-section .socials a {
  font-size: 1.2em;
  color: #ff3a6d;
}

.footer-section .socials a:hover {
  transform: translateY(-5px);
  color: #fff;
}

.footer-section .links ul {
  list-style: none;
}

.footer-section .links ul a {
  color: #fff;
  text-decoration: none;
  margin-bottom: 10px;
  display: inline-block;
  transition: transform 0.3s;
}

.footer-section .links ul a:hover {
  text-decoration: underline;
  transform: translateX(5px);
}

.footer-section .contact-form .text-input {
  background: #444;
  border: 1px solid #777;
  padding: 10px;
  width: calc(100% - 22px);
  color: #fff;
  margin-bottom: 10px;
  transition: background 0.5s, border-color 0.5s;
}

.footer-section .contact-form .text-input:focus {
  background: #555;
  border-color: #ff3a6d;
}

.footer-section .contact-form .btn {
  background: #ff3a6d;
  color: #fff;
  padding: 10px 20px;
  border: none;
  cursor: pointer;
  transition: background 0.5s, transform 0.3s;
}

.footer-section .contact-form .btn:hover {
  background: #ff5a8d;
  transform: translateY(-3px);
}

.footer-bottom {
  margin-top: 20px;
  border-top: 1px solid #777;
  padding: 20px 0;
}

@keyframes fadeIn {
  0% { opacity: 0; }
  100% { opacity: 1; }
}
</style>
