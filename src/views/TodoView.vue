<template>
  <h1>This is Todo page</h1>

  <h2>Add Todo</h2>
  <input type="text" v-model="newTodo" />
  <button @click="addTodo">Add</button>

  <h2>Todo List</h2>
  <ul>
    <li v-for="todo in todos" :key="todo">{{ todo }}</li>
  </ul>
</template>

<style scoped></style>

<script>
export default {
  data() {
    return {
      newTodo: '',
      todos: []
    }
  },
  methods: {
    addTodo() {
      this.todos.push(this.newTodo)
      this.newTodo = ''
    }
  }
}
</script>
