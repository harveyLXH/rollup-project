<template>
  <div class="app">
    <h2>App计算器: {{ count }}</h2>
    <button @click="increment">+1</button>
    <button @click="decrement">-1</button>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const count = ref(100)
function decrement() {
  count.value--
}
function increment() {
  count.value++
}
</script>

<style scoped></style>
