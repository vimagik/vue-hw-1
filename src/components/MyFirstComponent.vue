<script setup>
import { ref } from 'vue'

const clickStatus = ref(false)

function clickButton() {
  clickStatus.value = !clickStatus.value
}
</script>

<template>
  <h1>Первое ДЗ из курса по VUE</h1>
  <button @click="clickButton">Нажми меня</button>
  <p v-if="clickStatus">Cюрпиз</p>
</template>
