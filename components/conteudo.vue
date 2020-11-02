<template>
  <main>
    <carousel></carousel>
    <div class="container-fluid">
      <div class="row">
        <div class="row col-12 justify-content-center">
          <h1>Bem-vindo ao Vilo Vincenzzi!</h1>
        </div>

        <div class="row">
          <div class="container">
            <card
              titulo="Essa é nossa escola"
              imagem-alt="Descrição do card"
              texto="Olá Bem-vindo a nossa escola!"
            ></card>

            <card
              titulo="Nosso objetivo"
              imagem-alt="Descrição do card"
              texto="Lorem ipsum dolor sit amet consectetur adipisicing elit. Praesentium in officiis voluptas. Quam, laudantium? Nemo reprehenderit autem ratione veritatis doloribus recusandae quidem consectetur repellendus, velit sunt cupiditate, praesentium optio eius?"
            ></card>

            <card
              titulo="Nossa história"
              imagem-alt="Descrição do card"
              texto="Lorem ipsum dolor sit amet consectetur adipisicing elit. Praesentium in officiis voluptas. Quam, laudantium? Nemo reprehenderit autem ratione veritatis doloribus recusandae quidem consectetur repellendus, velit sunt cupiditate, praesentium optio eius?"
            ></card>
          </div>
        </div>
      </div>
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