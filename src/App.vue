<script setup lang="ts">
import { ref } from 'vue'
import JustGreeter from './component/JustGreeter.vue'

const message = ref<string>('')

function eventHandler(justValue: string) {
  alert(justValue)
}
</script>

<template>
  <h1>Vue reactive 실습</h1>
  <input v-model="message" placeholder="값 입력!" />
  <p>당신이 입력한 메시지 : {{ message }}</p>
  <JustGreeter :name="message" @update="eventHandler"></JustGreeter>
</template>

<style scoped></style>
