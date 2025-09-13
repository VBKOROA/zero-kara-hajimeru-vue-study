<script setup lang="ts">
import { ref } from 'vue'

const count = ref<number>(0)

function increment() {
  count.value++
}
</script>

<template>
  <h1>Vue 반응성 테스트</h1>
  <p>현재 카운트: {{ count }}</p>
  <button @click="increment">Up Up!</button>
</template>

<style scoped></style>
