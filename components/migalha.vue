<template>
      <nav aria-label="breadcrumb" :class="migalha">
      <ol class="breadcrumb bloco-texto9 corfundo">
        <li class="breadcrumb-item"><a href="/">Página inicial</a></li>
        <li class="breadcrumb-item active" aria-current="page">Contato</li>
      </ol>
    </nav>
</template>

<script>
export default {
    name: 'migalha-pao',

    props: ['migalha']
}
</script>

<style>

</style>