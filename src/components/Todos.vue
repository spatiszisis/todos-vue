<template>
  <div>
    <h1>Todos</h1>
    <div class="todos">
      <div v-for="todo in allTodos" :key="todo.id" class="todo">
        <p>{{ todo.title }}</p>
      </div>
    </div>
  </div>
</template>

<script>
import { mapGetters } from "vuex";

export default {
  name: "Todos",
  computed: mapGetters(["allTodos"]),
};
</script>

<style>
</style>