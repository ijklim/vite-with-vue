<script setup>
import { ref } from 'vue'
import AppButton from './AppButton.vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
  <h1>{{ msg }}</h1>

  <div class="card">
    <button type="button" @click="count++">Click to increment count: {{ count }}</button>

    <AppButton @click="count++" />
  </div>
</template>

<style scoped>
.card {
  text-align: center;
}

:deep(button) {
  background-color: lightgreen;
  border: 1px solid darkgray;
  color: darkgreen;
  margin-bottom: 10px;
}

:deep(button:hover) {
  background-color: darkgreen;
  color: white;
}
</style>
