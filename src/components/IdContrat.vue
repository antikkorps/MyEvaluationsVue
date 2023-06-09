<script setup>
import { ref } from 'vue'

const picker = ref(new Date().toISOString().substr(0, 10))
</script>
<template>
  <div>
    <v-sheet width="100%">
      <v-select
        label="Client"
        :items="['BNP', 'Crédit Agricole', 'SG', 'Bred']"
        variant="solo"
      ></v-select>

      <v-select
        label="Numéro de Contrat"
        :items="['2023-003', '2023-004', '2023-005', '2023-006']"
        variant="solo"
      ></v-select>

      <v-date-picker v-model="picker"></v-date-picker>
    </v-sheet>
  </div>
</template>
