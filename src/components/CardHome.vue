<script setup>
import { RouterLink } from 'vue-router'
</script>

<template>
  <div>
    <v-sheet
      class="d-flex align-center justify-center flex-wrap text-center mx-auto px-12"
      elevation="4"
      height="250"
      rounded
      max-width="800"
      width="100%"
    >
      <div>
        <h2 class="text-h4 font-weight-black text-orange">
          Bienvenue sur le site de vos évaluations!
        </h2>

        <div class="text-h5 font-weight-medium mb-2">
          Vous êtes sur le site des évaluations du Training Center
        </div>

        <p class="text-body-2 mb-4">Avant toute chose, vous devez vous connecter</p>

        <v-btn variant="text" color="orange" href="/about">Se connecter</v-btn>
      </div>
    </v-sheet>
  </div>
</template>
