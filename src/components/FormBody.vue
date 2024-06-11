<template>
  <section class="form-container">
    <h2>Formulario - Cuerpo</h2>
    <form>
      <div class="input-group">
        <input type="email" placeholder="Correo Electrónico" />
        <i class="fas fa-envelope"></i>
      </div>
      <div class="input-group">
        <textarea placeholder="Mensaje"></textarea>
        <i class="fas fa-comment"></i>
      </div>
      <button type="submit">Enviar</button>
    </form>
  </section>
</template>

<script>
export default {
  name: 'FormBody'
}
</script>

<style scoped>
.form-container {
  max-width: 400px;
  margin: 50px auto;
  padding: 50px;
  background-color: #222; /* Cambiado a negro */
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.4); /* Ajuste en la sombra */
  color: #fff; /* Cambiado el color del texto a blanco */
}

h2 {
  font-size: 24px;
  margin-bottom: 20px;
  text-align: center;
}

form {
  display: flex;
  flex-direction: column;
}

.input-group {
  position: relative;
  margin-bottom: 20px;
}

input,
textarea {
  width: 100%;
  padding: 10px;
  border: 1px solid #555; /* Cambiado el color del borde */
  border-radius: 4px;
  outline: none;
  font-size: 16px;
  background-color: #333; /* Cambiado el color de fondo */
  color: #fff; /* Cambiado el color del texto a blanco */
}

input:focus,
textarea:focus {
  border-color: #007bff;
}

i {
  position: absolute;
  top: 50%;
  right: 10px;
  transform: translateY(-50%);
  color: #aaa;
}

button {
  background-color: #007bff;
  color: #fff;
  border: none;
  border-radius: 4px;
  padding: 12px 20px;
  font-size: 16px;
  cursor: pointer;
  transition: background-color 0.3s;
}

button:hover {
  background-color: #0056b3;
}

/* Animaciones */
@keyframes slideInFromLeft {
  from {
    transform: translateX(-100%);
    opacity: 0;
  }
  to {
    transform: translateX(0);
    opacity: 1;
  }
}

@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

.form-container,
h2,
.input-group,
button {
  animation: slideInFromLeft 0.5s ease-out;
}

input,
textarea {
  animation: fadeIn 0.5s ease-out;
}
</style>
