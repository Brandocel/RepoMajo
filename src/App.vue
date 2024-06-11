<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Form />
    <Body />
    <Footer />
  </div>
</template>

<script>
import Form from './components/FormHeader.vue'
import Body from './components/FormBody.vue'
import Footer from './components/FormFooter.vue'

export default {
  name: 'App',
  components: {
    Form,
    Body,
    Footer
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
