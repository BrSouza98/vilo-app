<template>
 <div class="cardConfig">
    <b-card-group deck>
      <b-card header="titulo" alt="imagem-alt">
        <b-card-text>{{texto}}</b-card-text>
      </b-card>

    </b-card-group>
  </div>
</template>

<script>
export default {
  name: 'card',

  props: ['titulo', 'imagem-alt', 'texto'],

  data(){
    return{

    }
  }
};
</script>

<style scoped>
  .cardConfig{
    width: 400px;
    margin: 20px;
  }
</style>