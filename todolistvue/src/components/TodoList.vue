<template>
  <div>
    <TodoInputText v-model="newTodo" @keydown.enter="addTodo" />
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
      todos: ["Salade", "Tomates", "Oignons"],
      newTodo: ""
    };
  },

  methods: {
    addTodo() {
      const trimmedText = this.newTodo.trim();
      const capitalizeText =
        trimmedText.charAt(0).toUpperCase() +
        trimmedText.substr(1).toLowerCase();
      if (capitalizeText) {
        this.todos.push(capitalizeText);
        this.newTodo = "";
      }
    }
  }
};
</script>

<style>
</style>