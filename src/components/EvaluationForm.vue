<script setup>
import { ref } from 'vue'
import IdContrat from '../components/IdContrat.vue'
import Participant from '../components/Participant.vue'
import Notation from '../components/Notation.vue'

const tab = ref('id_contrat')
</script>

<template>
  <div class="container">
    <h2>Votre évaluation</h2>
    <div class="menu">
      <v-card>
        <v-tabs v-model="tab" bg-color="primary">
          <v-tab value="id_contrat">Identification contrat</v-tab>
          <v-tab value="participant">Participant</v-tab>
          <v-tab value="notation">Notation</v-tab>
        </v-tabs>

        <v-card-text>
          <v-window v-model="tab">
            <v-window-item value="id_contrat">
              <h3>Contrat</h3>
              <IdContrat />
            </v-window-item>

            <v-window-item value="participant">
              <h3>Section participant</h3>
              <Participant />
            </v-window-item>

            <v-window-item value="notation">
              <h3>Section notation</h3>
              <Notation />
            </v-window-item>
          </v-window>
        </v-card-text>
      </v-card>
    </div>
  </div>
</template>

<style scoped>
.container {
  width: 80%;
  justify-content: center;
  align-items: center;
  margin: 5em auto;
}

.container h2 {
  font-size: 2.5em;
  margin-bottom: 1em;
}

.container h3 {
  margin: 1em 0;
}
</style>
