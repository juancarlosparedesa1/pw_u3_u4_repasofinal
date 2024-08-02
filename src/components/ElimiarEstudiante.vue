<template>
  <div class="container">
    <h1>ElimiarEstudiante</h1>
    <p type="Cedula"><input type="text" v-model="cedula" /></p>
    <button v-on:click="borrar">Eliminar</button>
    <p v-if="mensaje">{{ mensaje }}</p>
  </div>
</template>

<script>
import { eliminarPorCedulaFachada } from "../clients/clienteEstudiante.js";
export default {
  data() {
    return {
      cedula: "",
      mensaje: "",
    };
  },
  methods: {
    async borrar() {
      const data = await eliminarPorCedulaFachada(this.cedula);
      console.log("Estudiante eliminado con exito");
      this.mensaje = "Estdudiante eliminado con exito";
    },
  },
};
</script>

<style>
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
p:before {
  content: attr(type);
  display: block;
}
p {
  text-align: left;
  margin-bottom: 0px;
}
input {
  margin-bottom: 0px;
}
h1 {
  margin-bottom: 0px; /* Ajusta según sea necesario */
}
button {
  margin-top: 20px;
}
</style>