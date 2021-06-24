<template>
  <div id="app" class="divapp">
    <img src="./assets/logo.png">
    <h1>{{ msg }}</h1>
    <test-component></test-component>
    <task-list-component></task-list-component>
  </div>
</template>

<script>

import TestComponent from './components/TestComponent'
import TaskListComponent from './components/TaskListComponent'

export default {
  name: 'app',
  data () {
    return {
      msg: 'Curso de vuejs'
    }
  },
  components: {
    TestComponent,
    TaskListComponent
  }
}
</script>

<style>

.divapp{
  border: 1px solid #42b983;
  margin: 5px;
  padding: 10px;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
