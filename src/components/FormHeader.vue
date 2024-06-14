<template>
  <div class="card">
    <header class="form-header">
      <div class="header-content">
        <h1>Formulario de Registro</h1>
        <p>Completa los campos a continuación para registrarte</p>
        <form>
          <input type="text" placeholder="Nombre" class="form-input" />
          <input type="email" placeholder="Correo electrónico" class="form-input" />
          <input type="password" placeholder="Contraseña" class="form-input" />
        </form>
      </div>
    </header>
  </div>
</template>

<script>
export default {
  name: 'FormHeader'
}
</script>

<style scoped>
.card {
  max-width: 600px;
  margin: 20px auto;
  border-radius: 10px;
  overflow: hidden;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.form-header {
  background-image: url('https://wallpapers.com/images/featured-full/aesthetic-iphone-8k436w42fxqrt0xb.jpg');
  background-size: cover;
  background-position: center;
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  text-align: center;
  padding: 40px 20px; /* Aumenté el padding para que el fondo sea visible alrededor del formulario */
}

.form-header::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.5); 
}

.header-content {
  position: relative;
  z-index: 1;
  max-width: 400px; /* Limité el ancho máximo del contenido para centrarlo visualmente */
}

.header-content h1 {
  font-size: 3em;
  margin-bottom: 10px;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.8);
}

.header-content p {
  font-size: 1.5em;
  margin-bottom: 20px;
}

.form-input {
  padding: 15px;
  font-size: 1.2em;
  width: calc(100% - 30px);
  border: none;
  border-radius: 5px;
  margin: 10px auto;
  display: block;
  background-color: rgba(255, 255, 255, 0.8);
}

.form-input::placeholder {
  color: #999;
}
</style>
