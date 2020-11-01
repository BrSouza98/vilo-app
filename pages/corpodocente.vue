<template>
  <div>
    <div class="centro margem2">
      <h1>Corpo Docente</h1>
      <p><img class="img1" src="~/assets/lousa.png" alt=""></p>
      <h1>A equipe docente é constituída de professores regentes, devidamente habilitados.</h1>
    </div>
    <div class="mt-4">
      <h3 class="margem"><b>Daniela Henriques - Coordenadora</b></h3>
      <b-card
        img-src="~/assets/coordenadora.jpg"
        img-alt="Card image"
        img-left
        class="mb-3 margem"
      >
        <b-card-text>
          Some quick example text to build on the card and make up the bulk of
          the card's content.
        </b-card-text>
      </b-card>

      <h3 class="nomeDocentesDireita margem">Cléo Rezende - Berçarista</h3>
      <b-card class="margem" img-src="~/assets/prof1.jpg" img-alt="Card image" img-right>
        <b-card-text>
          Some quick example text to build on the card and make up the bulk of
          the card's content.
        </b-card-text>
      </b-card>
      <h3 class="margem">Sandra Bruno - Auxiliar de desenvolvimento infantil</h3>
      <b-card
        img-src="~/assets/prof2.jpg"
        img-alt="Card image"
        img-left
        class="mb-3 margem"
      >
        <b-card-text>
          Some quick example text to build on the card and make up the bulk of
          the card's content.
        </b-card-text>
      </b-card>

      <h3 class="nomeDocentesDireita margem">Rose Colla - Professora maternal 2</h3>
      <b-card class="margem" img-src="~/assets/prof4.jpg" img-alt="Card image" img-right>
        <b-card-text>
          Some quick example text to build on the card and make up the bulk of
          the card's content.
        </b-card-text>
      </b-card>
      <h3 class="margem">Ludimila Gambogi - Professora jardim 1</h3>
      <b-card
        img-src="~/assets/ludimila.jpg"
        img-alt="Card image"
        img-left
        class="mb-3 margem"
      >
        <b-card-text>
          Some quick example text to build on the card and make up the bulk of
          the card's content.
        </b-card-text>
      </b-card>

      <h3 class="nomeDocentesDireita margem">Danilo Reinol - Professor jardim 2</h3>
      <b-card class="margem" img-src="~/assets/prof3.jpg" img-alt="Card image" img-right>
        <b-card-text>
          Some quick example text to build on the card and make up the bulk of
          the card's content.
        </b-card-text>
      </b-card>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.nomeDocentesDireita {
  text-align: right;
}
img {
  border-radius: 100%;
  width: 200px;
  height: 200px;
}
.img1{
 width: 350px;
 height: 350px;
}
.margem{
  margin-top: 30px;
}
.margem2{
  margin-top: 50px;
}
.centro{
  text-align: center;
}
.cor{
  background-color:blue;
}
</style>