<template>
  <div>
    <AddTodo></AddTodo>
    <filter-todos></filter-todos>
    <Todos></Todos>
  </div>
</template>

<script>
import Todos from './components/Todos.vue'
import AddTodo from './components/AddTodo.vue'
import FilterTodos from "./components/FilterTodos";
export default {
  name: 'App',
  components: {
    Todos,
    AddTodo,
    FilterTodos
  }
}
</script>

<style>
</style>
