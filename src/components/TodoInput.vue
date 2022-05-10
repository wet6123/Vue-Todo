<template>
  <div>
    <input
      type="text"
      v-model="newTodo"
      placeholder="해야할 일을 입력해주세요."
      @keyup.enter="addTodo"
    />
    <button class="addContainer" @click="addTodo">+</button>

    <AlertModal v-if="showModal" @close="showModal = false">
      <template v-slot:header>
        <h3>경고</h3>
      </template>
      <template v-slot:body>
        <span>해야할 일을 입력해주세요!</span>
      </template>
      <template v-slot:footer>
        <button @click="showModal = false">닫기</button>
      </template>
      <span>해야할 일을 입력해주세요!</span>
    </AlertModal>
  </div>
</template>

<script>
import AlertModal from "./common/AlertModal.vue";

export default {
  components: {
    AlertModal,
  },
  data() {
    return {
      showModal: false,
    };
  },
};
</script>
