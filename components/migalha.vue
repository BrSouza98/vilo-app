<template>
  <nav aria-label="breadcrumb" v-show="Mensagem">
    <ol class="breadcrumb">
      <li class="breadcrumb-item"><a href="/">Página inicial</a></li>
      <li class="breadcrumb-item active" aria-current="page">Contato</li>
      <li class="breadcrumb-item">
        <p>{{ Mensagem }}</p>
      </li>
    </ol>
  </nav>
</template>

<script>
import conteudoVue from "./conteudo.vue";
export default {
  name: "migalha",

  data() {
    return {
      Mensagem: true,
    };
  },

  components: {
    conteudo: conteudoVue,
  },
};
</script>

<style scoped>
.breadcrumb {
  background-color: white;
}
</style>