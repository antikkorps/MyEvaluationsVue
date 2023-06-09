<script setup>
import { RouterLink } from 'vue-router'
</script>
<template>
  <div>
    <v-container>
      <v-row justify="center">
        <v-col cols="auto">
          <RouterLink to="/evaluations">
            <v-btn :ripple="false"> Mes évaluations </v-btn>
          </RouterLink>
        </v-col>

        <v-col cols="auto">
          <RouterLink to="/results">
            <v-btn :ripple="false"> Mes résultats </v-btn>
          </RouterLink>
        </v-col>

        <v-col cols="auto">
          <RouterLink to="/evaluation-form">
            <v-btn :ripple="false"> Création de formulaire </v-btn>
          </RouterLink>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
