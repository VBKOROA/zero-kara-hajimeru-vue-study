<script setup lang="ts">
import { ref } from 'vue'

const message = ref<string>('')
</script>

<template>
  <h1>Vue reactive 실습</h1>
  <input v-model="message" placeholder="값 입력!" />
  <p>당신이 입력한 메시지 : {{ message }}</p>
</template>

<style scoped></style>
