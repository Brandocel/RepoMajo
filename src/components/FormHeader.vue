<template>
    <header class="form-header">
      <div class="header-content">
        <h1>Formulario de Registro</h1>
        <p>Completa los campos a continuación para registrarte</p>
        <input type="text" placeholder="Nombre" class="form-input" />
      </div>
    </header>
  </template>
  
  <script>
  export default {
    name: 'FormHeader'
  }
  </script>
  
  <style scoped>
  .form-header {
    background-image: url('https://wallpapers.com/images/featured-full/aesthetic-iphone-8k436w42fxqrt0xb.jpg');
    background-size: cover;
    background-position: center;
    position: relative;
    height: 50vh; 
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    text-align: center;
    padding: 20px;
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
  }
  
  .header-content h1 {
    font-size: 3em;
    margin-bottom: 10px;
  }
  
  .header-content p {
    font-size: 1.5em;
    margin-bottom: 20px;
  }
  
  .form-input {
    padding: 15px;
    font-size: 1.2em;
    width: 80%;
    max-width: 400px;
    border: none;
    border-radius: 5px;
    margin-top: 10px;
  }
  
  .form-input::placeholder {
    color: #ccc;
  }
  </style>
  