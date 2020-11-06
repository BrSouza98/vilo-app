<template>
  <div>
    <carousel></carousel>
    <conteudo></conteudo>
  </div>
</template>

<script>
import migalhaVue from "../components/migalha.vue";

export default {
  components: {
    migalhaComponent: migalhaVue,
  },

  data() {
    return {
      migalha: "d-none",
    };
  },
};
</script>

<style scoped>
</style>