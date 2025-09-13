<script setup lang="ts">
import { reactive } from 'vue'

interface User {
  name: string
  age: number
}

const user = reactive<User>({
  name: 'abko',
  age: 1,
})

function celebrateBirth() {
  user.age++
}
</script>

<template>
  <h1>Vue reactive 실습</h1>
  <p>이름 : {{ user.name }}</p>
  <p>나이 : {{ user.age }}</p>
  <button @click="celebrateBirth">나이 추가요~</button>
</template>

<style scoped></style>
