<template>
  <div>
    <!--  
   navegacion tradicional 
    <a href="/ingresar">Insertar</a>
    <a href="/consultarActualizar">Consultar-Actualizar</a>
    <a href="eliminar">Eliminar</a> -->
    <router-link to="/ingresar">Insertar</router-link>
    <router-link to="/consultarActualizar/vacio">Consultar-Actualizar</router-link>
    <router-link to="/eliminar">Eliminar</router-link>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
div {
  padding: 0px 30px;
}
/* combinacion jerarquica
    solo a los elemntos a que tenga como padre un div
 */
div a {
  color: black;
  margin: 0px 10px;
  border: 1px solid black;
}
</style>