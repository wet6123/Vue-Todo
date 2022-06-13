<template>
  <v-container>
    TodoInput
    <v-form>
      <v-container>
        <v-row>
          <v-col cols="12">
            <v-text-field
              v-model="newTodo"
              :rules="nameRules"
              label="Input To-Do"
            ></v-text-field>
          </v-col>
        </v-row>
      </v-container>
    </v-form>
  </v-container>
</template>

<script>
export default {
  name: "TodoInput",
};
</script>

<style></style>
