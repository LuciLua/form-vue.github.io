<template>
  <form style="display: flex; flex-direction: column; max-width: 500px">
    <label for="Nome">Nome do aluno</label>
    <input placeholder="Nome do aluno" />
    <label for="Nome">Matricula do aluno</label>
    <input placeholder="Matricula do aluno" />
    <label for="Nome">Senha do aluno</label>
    <input placeholder="Senha do aluno" />
    <button style="margin-top: 10px">Cadastrar Aluno</button>
  </form>
  <!-- {{ msg }} -->
</template>

<script>
export default {
  name: "FormularioAlunos",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

label{
  font-size: 13px;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  margin-bottom: 2px;
  width: 100%;
  text-align: start;
}

input {
  padding: 8px 5px;
  border: none;
  border-radius: 2px;
  margin-bottom: 20px;

  outline: none;
}

button {
  border-radius: 2px;
  padding: 10px;
  border: none;
  background: #415b76;
  color: #fff;
  cursor: pointer;
}
</style>
