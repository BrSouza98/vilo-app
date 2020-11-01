<template>
  <div class="menu">
    <div>
      <b-navbar toggleable="lg" type="dark" variant="info">
        <b-navbar-brand href="/">Vilo Vincenzzi</b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <!-- Right aligned nav items -->
          <b-navbar-nav class="ml-auto">
            <b-navbar-nav>
              <b-nav-item href="sobre">Sobre</b-nav-item>
              <b-nav-item href="turmas">Turmas</b-nav-item>
              <b-nav-item href="corpodocente">Corpo Docente</b-nav-item>
              <b-nav-item href="blog">Blog</b-nav-item>
              <b-nav-item href="contato">Contatos</b-nav-item>
            </b-navbar-nav>
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>