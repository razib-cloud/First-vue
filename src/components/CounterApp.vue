<script setup>
import { ref } from "vue";

let count = ref(0);
const increase = () => count.value++;
const decrease = () => count.value--;
</script>

<template>
  <h1>Counter</h1>

  <p>Value {{ count }}</p>
  <button @click="increase">Plus</button>
  <button @click="decrease">Minus</button>
</template>

<style scoped></style>
