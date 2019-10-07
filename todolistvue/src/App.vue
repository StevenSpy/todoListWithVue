<template>
  <div id="app" class="container">
    <h1 class="title is-1">Hello World !</h1>
    <TodoList />
  </div>
</template>

<script>
import TodoList from "@/components/TodoList.vue";
export default {
  name: "app",
  components: {
    TodoList
  }
};
</script>

<style lang="scss">
#app {
  margin: 60px 60px 0 100px;
}
.input {
  width: 50vw;
}
</style>
