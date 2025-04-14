<script setup lang="ts">
import { Button } from "@progress/kendo-vue-buttons";

defineProps<{ msg: string }>()
</script>

<template>
  <h1>{{ msg }}</h1>
  <div class="card">
    <button type="button">Regular button</button>
    <button class="btn btn-primary">Bootstrap Button</button>
    <Button themeColor="primary">Kendo Button</Button>
  </div>
</template>

<style scoped>
  .card {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 10px; /* Adds spacing between buttons */
    height: fit-content;
    padding: 25px;
  }
</style>

