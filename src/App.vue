<template>
  <Header />
  <!-- <About /> -->
  <Habilidades />
  <Contacto />
  <Footer />
</template>

<script>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import Contacto from "./components/Contacto.vue";
import Habilidades from "./components/Habilidades.vue";
// import About from "./components/About.vue";

export default {
  name: "App",
  created() {
    document.title = "Abel Heredia Bravo";
  },
  components: {
    Header,
    Footer,
    Contacto,
    Habilidades,
    // About,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
