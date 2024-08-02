<template>
  <!-- <EstudiantesPage /> -->
  <!-- <BienvenidaPage /> -->
  <navBar />
  <router-view />
</template>

<script>
/* import EstudiantesPage from "./Pages/EstudiantesPage.vue"; */
/* import BienvenidaPage from "./Pages/BienvenidaPage.vue";
 */
import navBar from "./components/navBar.vue";

export default {
  name: "App",
  components: {
    navBar,
    /*  BienvenidaPage, */
    /* EstudiantesPage, */
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
  margin-top: 60px;
}
</style>
