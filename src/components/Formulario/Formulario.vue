<template>
  <form class="form">
    <div class="c_input">
      <input required value="" id="nome" />
      <label for="nome">Nome do aluno</label>
    </div>
    <div class="c_input">
      <input required value="" id="matricula" />
      <label for="matricula">Matricula do aluno</label>
    </div>
    <div class="c_input">
      <input type="password" required value="" id="senha" />
      <label for="senha">Senha do aluno</label>
    </div>
    <button type="reset" @click="showModal();">Cadastrar Aluno</button>
  </form>
  <ModalAlerts msg="Aluno cadastrado com sucesso!" v-if="modal" />
</template>

<script>
import ModalAlerts from "../Modal/Modal.vue";

export default {
  name: "FormularioAlunos",
  props: {
    msg: String,
  },
  components: {
    ModalAlerts,
  },
  data: function () {
    return {
      modal: false,
    };
  },
  methods: {
    showModal: function () {
      this.modal = true;
      setTimeout(() => {
        this.modal = false;
      }, 3000);
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url(style.css);
</style>
