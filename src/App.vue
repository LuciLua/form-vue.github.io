<template>
  <div
    style="
      width: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
    "
  >
    <h1 style="margin-bottom: 20px;">Formulário</h1>
    <FormularioAlunos msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
import FormularioAlunos from "./components/Formulario.vue";

export default {
  name: "App",
  components: {
    FormularioAlunos,
  },
};
</script>

<style>
*::before,
*,
*::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-content: center;
  flex-direction: column;

  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #c1cfde;
  background-color: #2c3e50;
}
</style>
