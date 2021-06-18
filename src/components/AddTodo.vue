<template>
  <div>
    <h3>AddTodo</h3>
    <div>
      <form @submit="onSubmit">
        <input type="text" v-model="title" placeholder="Add Todo...">
        <input type="submit" value="Submit">
      </form>
    </div>
  </div>
</template>
<script>
import {mapActions} from 'vuex'
export default {
  name: "AddTodo",
  data() {
    return {
      title:''
    }
  },
  methods: {
    ...mapActions(['addTodo']),
    onSubmit(e) {
      e.preventDefault();
      this.addTodo(this.title);
    }
  }
}
</script>
<style scoped>

</style>