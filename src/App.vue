<template>
  <div id="app" class="container">
    <h1 class="text-center">Todo App</h1>
    <form @submit.prevent="addTodo()">
  <div class="form-group">
    <label for="newTodo">New Todo:</label>
        <small id="newTodoHelp" class="form-text text-muted">Enter a new todo</small>
    <input type="text" class="form-control" id="newTodo" aria-describedby="newTodoHelp" placeholder="Walk the dawg!">
  </div>
  <button type="submit" class="btn btn-primary">Add Todo</button>
</form>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      newTodo: ''
    }
  },
  methods: {
    addTodo() {
      console.log('form submitted!')
    },
  }
}
</script>

<style>
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
