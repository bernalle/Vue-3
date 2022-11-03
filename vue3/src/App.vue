<template>
  <div id="app">
    <h1>Bem vindo ao primeiro projeto!</h1>
    <p>Componente App:{{nome}} </p>

    <button @click="entrar">Entrar</button>
   
    <Usuario :nome="nome" @cursoNovo="nome = $event"/>

  </div>
</template>

<script>
import Usuario from './components/Usuario.vue'

export default {
  name: 'App',
  components: {
    Usuario,
  },
  data() {
    return {
      nome: 'Sujeito programador'
    }
  },
  methods: {
    entrar() {
      this.nome = "Mudou o nome";
      // alert("Mudou o nome");}  
    }
  }
}
</script>

<style>

</style>