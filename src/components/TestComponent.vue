<template>
  <div class="divtest">
    <h3>{{ title }}</h3>
    <p>{{ msg }}</p>
    <form-component></form-component>
  </div>
</template>

<script>
import FormComponent from './FormComponent'

export default {

  data() {
    return {
      msg: 'Teste de componentes.',
      title : 'Test Component'
    }
  },
  components: {
    FormComponent
  }
}
</script>

<style scoped>
.p{
  color: aquamarine;
}
.divtest{
  border: 1px solid #42b977;
  margin: 5px;
  padding: 10px;
}
</style>


