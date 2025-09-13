<script setup lang="ts">
defineProps<{
  name?: string
}>()

const emit = defineEmits<{
  (e: 'update', justValue: string): void
}>()

function eventEmit() {
  emit('update', '와라라라랄')
}
</script>

<template>
  <div class="greeting-box">
    <p>안녕하세요! {{ name }}님! 환영합니다~~</p>
    <button @click="eventEmit">눌러보기!</button>
  </div>
</template>

<style scoped>
.greeting-box {
  width: 16rem;
  height: 6rem;
  background-color: burlywood;
  border-radius: 0.4rem;
  padding: 0 0.4rem;
}
</style>
