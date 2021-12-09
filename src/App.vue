
<template>
  <div id="app">
    <navigation/>
    <perfil/>
    <about/>
    <projects/>
    <skills/>
    <contact/>
  </div>
</template>

<script>
import Navigation from './components/Navigation.vue'
import Perfil from './components/Perfil.vue'
import About from './components/About.vue'
import Projects from './components/Projects.vue'
import Skills from './components/Skills.vue'
import Contact from './components/Contact.vue'

export default {
  name: 'App',
  components: {
    Navigation,
    Perfil,
    About,
    Projects,
    Skills,
    Contact
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins&display=swap');

#app {
  
  font-family: 'Poppins', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
