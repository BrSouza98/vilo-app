<template>
  <main>
    <div>
      <div class="d-flex justify-content-center">
        <h1>Bem-vindo ao Vilo Vincenzzi!</h1>
        <h1 class="animate__animated animate__bounce">An animated element</h1>

      </div>

      <b-container fluid>
        <b-row>
          <b-col cols="4">
            <card
              titulo="Essa escolinha é pika!"
              imagem-alt="Descrição do card"
              texto="Lorem ipsum dolor sit amet consectetur adipisicing elit."
              class="animate__animated animate__fadeInLeft"
            ></card>
          </b-col>


          <b-col cols="4">
            <card
              titulo="Essa escolinha é pika!"
              imagem-alt="Descrição do card"
              texto="Lorem ipsum dolor sit amet consectetur adipisicing elit."
              class="animate__backInUp"
            ></card>
          </b-col>

          <b-col cols="4">
            <card
              titulo="Essa escolinha é pika!"
              imagem-alt="Descrição do card"
              texto="Lorem ipsum dolor sit amet consectetur adipisicing elit."
              class="animate__backInRight"
            ></card>
          </b-col>

        </b-row>
        
      </b-container>
    </div>

    <footer></footer>
  </main>
</template>

<script>
import cardVue from "./card.vue";
export default {
  components: {
    card: cardVue,
  },
};
</script>

<style scoped>
</style>