<script setup>
import { ref } from "vue";
import { Tests } from "easy-coms-vite";
defineProps({
  msg: String,
});

const count = ref(0);
</script>

<template>
  <div>
    <h1>{{ msg }}</h1>
    <a-button>外部的按钮</a-button>
    <Tests />
  </div>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
