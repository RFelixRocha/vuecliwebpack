<template>
  <div class="divtask">
    <h3>{{ title }}</h3>
    <ul v-for="(task, index) in tasks" :key="index">
      <li :class="task.completed ? 'active':'no-active'">{{ task.name }}</li>
    </ul>
  </div>
</template>

<script>

export default {
  data() {

    return {

      tasks: [
        {name: 'lista 01', completed: true},
        {name: 'lista 02', completed: true},
        {name: 'lista 03', completed: false},
        {name: 'lista 04', completed: true},
        {name: 'lista 05', completed: false}
      ],
      title : 'Task Component'

    }

  },
}

</script>

<style scoped>

.divtask{
  border: 1px solid #426cb9;
  margin: 5px;
  padding: 10px;
}
.active{
  color: green;
}
.no-active{
  color: red;
}

</style>
