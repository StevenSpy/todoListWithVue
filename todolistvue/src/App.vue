<template>
  <div id="app">
    <h1 class="title is-1">Ma To Do List</h1>
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
  margin: 100px 100px 0 100px;
}
h1{
  text-align: center;
}
</style>
