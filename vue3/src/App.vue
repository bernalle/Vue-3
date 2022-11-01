<template>
  <div id="app">
    <h1>Bem vindo ao primeiro projeto!</h1>
    <Usuario/>
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
        nome:'Sujeito programador'
      }
    },
  }
</script>

<style>

</style>