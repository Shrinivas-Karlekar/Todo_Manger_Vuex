<template>
  <div>
    Filter Todos:
    <select @change="filterTodos($event)">
      <option value="5">5</option>
      <option value="3">3</option>
    </select>
  </div>
</template>

<script>
import {mapActions} from 'vuex';
export default {
  name: 'FilterTodos',
  methods: mapActions(["filterTodos"])
}
</script>

<style>
</style>
