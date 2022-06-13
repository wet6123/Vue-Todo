<template>
  <v-app>
    <v-main>
      <HeaderBar />
      <TodoInput />
      <TodoList />
      <FooterBar />
    </v-main>
  </v-app>
</template>

<script>
import TodoInput from "./components/TodoInput.vue";
import TodoList from "./components/TodoList.vue";
import HeaderBar from "./components/HeaderBar.vue";
import FooterBar from "./components/FooterBar.vue";

export default {
  name: "App",

  components: {
    TodoInput,
    TodoList,
    HeaderBar,
    FooterBar,
  },

  data: () => ({
    //
  }),
};
</script>
