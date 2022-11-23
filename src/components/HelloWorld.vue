<script setup>
import { ref } from 'vue'

defineProps({
  msg: String
})

const displayMsg = ref('')

function handleClick() {
  displayMsg.value = 'Element Plus imported successfully'
}
</script>

<template>
  <h2>{{ msg }}</h2>
  <el-button type="primary" @click="handleClick">Test</el-button>
  <div>{{ displayMsg }}</div>
</template>

<style scoped></style>
