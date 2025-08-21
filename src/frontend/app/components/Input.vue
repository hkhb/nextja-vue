<script setup lang="ts">
import { ref } from 'vue'

defineProps<{ msg: string }>()

const number = ref()
const readnumber = () => {
  return "12345678901234"
} 
const sendnumber = () => {
  console.log("send number", number.value)
}

</script>

<template>
  <button @click="readnumber">Click Me</button>
  <input type="text" v-model = number>
  <button @click="sendnumber"></button>
</template>

<style scoped>
</style>
