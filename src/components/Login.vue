<template>
  <div id="login">
    <h1>로그인 페이지 입니다!.</h1>
    <button @click="todo()">click?</button>
    <router-link :to="'todoapp'">router-link</router-link>
    <a href="todoapp">click?</a>
  </div>
</template>

<script>
import TodoApp from "./todo/TodoApp"
export default {
  name: 'login',
  methods: {
    todo () {
      this.$router.push({
        name: 'todo-app' //
      })
    }
  }
}
</script>

<style scoped>
.alert-danger p{  
  color: red;
}
</style>