<template>
  <main>
    <div class="container-fluid">
      <div class="row">
        <div class="row col-12 justify-content-center">
          <h1>Bem-vindo ao Vilo Vincenzzi!</h1>
        </div>

        <div class="row">
          <div class="container">
            <card
              localImagem="https://i0.wp.com/www.ambersistemas.com.br/wp-content/uploads/2017/09/dicas-para-captar-alunos-para-sua-escola-20170821133431.jpg.jpg?fit=1254%2C837&ssl=1"
              titulo="Essa escolinha é pika!"
              imagem-alt="Descrição do card"
              texto="Lorem ipsum dolor sit amet consectetur adipisicing elit."
            ></card>

            <card
              titulo="Nosso objetiescrição do vo"
              imagem-alt="Dcard"
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