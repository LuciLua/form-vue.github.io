<template>
  <div class="modal" v-if="modal">
    <div class="x" @click="closeModal()">X</div>
    <p>{{ msg }}</p>
  </div>
</template>
  
  <script>
export default {
  name: "ModalAlerts",
  props: {
    msg: String,
  },
  data: function () {
    return {
      modal: true,
    };
  },
  methods: {
    closeModal: function () {
      this.modal = false;
    },
  },
};
</script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
@import url(style.css);
</style>
  