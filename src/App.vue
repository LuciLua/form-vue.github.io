<template>
  <div class="c_form">
    <h1>Cadastro de Alunos</h1>
    <FormularioAlunos msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
import FormularioAlunos from "./components/Formulario/Formulario.vue";

export default {
  name: "App",
  components: {
    FormularioAlunos,
  },
};
</script>

<style>
@import url("styles/globals.css");
</style>
