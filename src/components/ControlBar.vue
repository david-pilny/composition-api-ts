<script lang="ts" setup>
import { defineEmits } from 'vue'

const emit = defineEmits<{
  (event: 'add-number', num: number): void
  (event: 'reset-count'): void
}>()
</script>

<template>
  <button @click="emit('add-number', 1)">Add</button>
  <button @click="emit('reset-count')">Reset</button>
</template>
