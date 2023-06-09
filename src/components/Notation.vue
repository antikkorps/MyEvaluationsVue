<script setup>
import { ref } from 'vue'

const value = ref(0)
</script>
<template>
  <div>
    <v-slider
      v-model="value"
      color="orange"
      label="Name du field"
      :min="0"
      :max="5"
      :step="0.5"
      thumb-label
    ></v-slider>
  </div>
</template>

<style scoped></style>
