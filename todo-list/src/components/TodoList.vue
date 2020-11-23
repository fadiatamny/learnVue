<template>
  <div>
    <div v-bind:key="todo.id" v-for="todo in array">
      <Todo v-bind:data="todo" />
    </div>
  </div>
</template>
<script lang="ts">
import Vue from "vue";
import Todo from "./Todo.vue";

export default Vue.extend({
  name: "TodoList",
  components: {
    Todo
  },
  props: ["todos"],
  data: function() {
    return {
      array: [
        { id: 1, title: "test" },
        { id: 2, title: "test" },
        { id: 3, title: "test" },
        { id: 4, title: "test" }
      ]
    };
  }
});
</script>
<style scoped></style>
