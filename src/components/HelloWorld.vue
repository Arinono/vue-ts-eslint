<script setup lang="ts">
import { ref, Ref } from 'vue'

defineProps<{ msg: string }>()

const count: Ref<number> = ref(0)
</script>

<template>
  <h1>{{ msg }}</h1>
  new

  <div class="card">
    <button type="button" @click="count++">count is {{ count }}</button>
  </div>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
