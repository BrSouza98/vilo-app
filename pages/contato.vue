<template>
<div class="margem fundo">
  <div class="container">
  <div class="row">
    <div class="col">
     <div>
    <b-form @submit="onSubmit" @reset="onReset" v-if="show">
      <b-form-group
        id="input-group-1"
        label="Seu e-mail:"
        label-for="input-1"
      >
        <b-form-input
          id="input-1"
          v-model="form.email"
          type="email"
          required
          placeholder="Digite seu e-mail aqui."
        ></b-form-input>
      </b-form-group>

      <b-form-group id="input-group-2" label="Seu nome:" label-for="input-2">
        <b-form-input
          id="input-2"
          v-model="form.name"
          required
          placeholder="Digite seu nome aqui"
        ></b-form-input>
      </b-form-group>

      
      <b-form-group id="input-group-3" label="Assunto:" label-for="input-3">
        <b-form-select
          id="input-4"
          v-model="form.assunto"
          :options="assuntos"
          required
        ></b-form-select>
      </b-form-group>

  <div>
    <b-form-textarea
      id="textarea"
      placeholder="Escreva aqui a sua mensagem."
      rows="3"
      max-rows="3"
    ></b-form-textarea>

    <pre class="mt-3 mb-0">{{ text }}</pre>
  </div>

      <b-button type="submit" variant="primary">Enviar</b-button>
      <b-button type="reset" variant="danger">Apagar</b-button>
    </b-form>
    
  </div>
    </div>
    <div class="col">
      <h1>Fale conosco</h1>
      <p><svg width="1em" height="1em" viewBox="0 0 16 16" class="bi bi-house-fill" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
  <path fill-rule="evenodd" d="M8 3.293l6 6V13.5a1.5 1.5 0 0 1-1.5 1.5h-9A1.5 1.5 0 0 1 2 13.5V9.293l6-6zm5-.793V6l-2-2V2.5a.5.5 0 0 1 .5-.5h1a.5.5 0 0 1 .5.5z"/>
  <path fill-rule="evenodd" d="M7.293 1.5a1 1 0 0 1 1.414 0l6.647 6.646a.5.5 0 0 1-.708.708L8 2.207 1.354 8.854a.5.5 0 1 1-.708-.708L7.293 1.5z"/>
</svg> Av Cap. José Camargo Lima, 341, Jardim São Sebastião Taquaritinga/SP</p>
<p><svg width="1em" height="1em" viewBox="0 0 16 16" class="bi bi-telephone-plus-fill" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
  <path fill-rule="evenodd" d="M1.885.511a1.745 1.745 0 0 1 2.61.163L6.29 2.98c.329.423.445.974.315 1.494l-.547 2.19a.678.678 0 0 0 .178.643l2.457 2.457a.678.678 0 0 0 .644.178l2.189-.547a1.745 1.745 0 0 1 1.494.315l2.306 1.794c.829.645.905 1.87.163 2.611l-1.034 1.034c-.74.74-1.846 1.065-2.877.702a18.634 18.634 0 0 1-7.01-4.42 18.634 18.634 0 0 1-4.42-7.009c-.362-1.03-.037-2.137.703-2.877L1.885.511zM12.5 1a.5.5 0 0 1 .5.5V3h1.5a.5.5 0 0 1 0 1H13v1.5a.5.5 0 0 1-1 0V4h-1.5a.5.5 0 0 1 0-1H12V1.5a.5.5 0 0 1 .5-.5z"/>
</svg> (16) 3252-7799</p>
<p><svg width="1em" height="1em" viewBox="0 0 16 16" class="bi bi-envelope-fill" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
  <path fill-rule="evenodd" d="M.05 3.555A2 2 0 0 1 2 2h12a2 2 0 0 1 1.95 1.555L8 8.414.05 3.555zM0 4.697v7.104l5.803-3.558L0 4.697zM6.761 8.83l-6.57 4.027A2 2 0 0 0 2 14h12a2 2 0 0 0 1.808-1.144l-6.57-4.027L8 9.586l-1.239-.757zm3.436-.586L16 11.801V4.697l-5.803 3.546z"/>
</svg> vilovicenzzi@gmail.com</p>
<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3715.130333909059!2d-48.49759028679131!3d-21.38477219129913!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x94b939221cc723df%3A0xe809cd4ed3abc464!2sAv.%20Cap.%20Jos%C3%A9%20Camargo%20de%20Lima%2C%20431%20-%20Vila%20S%C3%A3o%20Sebasti%C3%A3o%2C%20Taquaritinga%20-%20SP%2C%2015900-000!5e0!3m2!1spt-BR!2sbr!4v1604199025720!5m2!1spt-BR!2sbr" width="600" height="450" frameborder="0" style="border:0;" allowfullscreen="" aria-hidden="false" tabindex="0"></iframe>
    </div>
  </div>
  </div>
  </div>
</template>

<script>
 export default {
    data() {
      return {
        form: {
          email: '',
          name: '',
          assunto: null,
          checked: []
        },
        assuntos: [{ text: 'Selecione o assunto.', value: null }, 'Aluno', 'Direção', 'Matriculas', 'Duvidas'],
        show: true
      }
    },
    methods: {
      onSubmit(evt) {
        evt.preventDefault()
        alert(JSON.stringify(this.form))
      },
      onReset(evt) {
        evt.preventDefault()
        // Reset our form values
        this.form.email = ''
        this.form.name = ''
        this.form.assunto = null
        this.form.checked = []
        // Trick to reset/clear native browser form validation state
        this.show = false
        this.$nextTick(() => {
          this.show = true
        })
      }
    }
  }
</script>

<style>
.margem{
  margin-top: 40px;
}
.centro{
  text-align: center;
}
.fundo{
  background-color:#fff;
}
</style>