<template>
  <div id="app">
    <h1 class="title">Hello World !</h1>
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
</style>
