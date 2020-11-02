<template>
  <div>
    <div>
      <b-navbar toggleable="lg" type="dark" variant="info">
        <b-navbar-brand href="/">Vilo Vincenzzi</b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <!-- Right aligned nav items -->
          <b-nav class="ml-auto">
            <b-nav>
              <b-nav-item href="sobre">Sobre</b-nav-item>
              <b-nav-item href="metodologia">Metodologia</b-nav-item>
              <b-nav-item href="corpodocente">Corpo Docente</b-nav-item>
              <b-nav-item href="https://vilovicenzzi.wordpress.com/" target="_blank">Blog</b-nav-item>
              <b-nav-item href="contato">Contatos</b-nav-item>
            </b-nav>
          </b-nav>
        </b-collapse>
      </b-navbar>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>

//regras do menu e interações
a {
  color: rgb(70, 70, 70);
  border-bottom: 3px solid rgb(255, 255, 255);
  box-sizing: content-box;
  margin: 5px;
  font-weight: 600;

  &:hover {
    animation-name: simple-border;
    animation-duration: 0.5s;
    animation-iteration-count: 1;
    animation-timing-function: ease-in;
    border-bottom-color: black;
    color: black;
    
  }

}

@keyframes simple-border {
  from {border-bottom-color: white;}
  to {border-bottom-color: black;}
}

//cor do menu
.bg-info {
  background-color: #ffffff !important;
}

.navbar-dark .navbar-brand {
  color: rgb(0, 0, 0);
}

</style>