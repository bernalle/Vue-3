<template>
  <div id="usuario">
    <h2> Olá Prop: {{nome}}</h2>
    <button @click="curso">Novo Curso</button>
  </div>
</template>

<script>
export default {
  name: 'Usuario',
  props: {
    nome: {
      type:String,
      required: false,
    }
  },
  methods: {
    curso() {
      var nome = "Curso de VueJS";
      this.$emit('cursoNovo', nome);
    }
  }
};

</script>

<style scoped>
  h2{
    color:red;
  }
</style>
