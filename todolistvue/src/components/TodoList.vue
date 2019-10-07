<template>
  <div>
    <TodoInputText v-model="newTodo" />
    <TodoListItem :todos="todos" />
  </div>
</template>

<script>
import TodoInputText from "@/components/TodoInputText.vue";
import TodoListItem from "@/components/TodoListItem.vue";
export default {
  components: {
    TodoInputText,
    TodoListItem
  },

  data() {
    return {
      todos: [Salade, Tomates, Oignons],
      newTodo: ""
    };
  }
};
</script>

<style>
</style>