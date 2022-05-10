<template>
  <section>
    <transition-group name="list" tag="ul">
      <li
        v-for="(todoItem, index) in propsdata"
        v-bind:key="todoItem"
        class="shadow"
      >
        <font-awesome-icon class="checkBtn" icon="check" aria-hidden="true" />
        {{ todoItem }}
        <span
          class="removeBtn"
          type="button"
          @click="removeTodo(todoItem, index)"
        >
          <button class="addBtn">삭제</button>
        </span>
      </li>
    </transition-group>
  </section>
</template>

<script>
export default {};
</script>

<style scoped></style>
