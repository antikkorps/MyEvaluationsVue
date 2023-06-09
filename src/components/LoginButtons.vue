<script setup>
import { RouterLink } from 'vue-router'
</script>
<template>
  <div>
    <v-container>
      <v-row justify="center">
        <v-col cols="auto">
          <RouterLink to="/login">
            <v-btn :ripple="false"> Se connecter </v-btn>
          </RouterLink>
        </v-col>

        <v-col cols="auto">
          <RouterLink to="/register">
            <v-btn :ripple="false"> s'inscrire </v-btn>
          </RouterLink>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
