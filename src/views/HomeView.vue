<script setup>
import { ref } from 'vue'
import LoginButtons from '@/components/LoginButtons.vue'
import MyDashboardLinks from '@/components/MydashboardLinks.vue'

const isLogin = ref(false)

const toggleLogin = () => {
  isLogin.value = !isLogin.value
}
</script>

<template>
  <main>
    <h1>Bienvenue sur le site de vos évaluations</h1>
    <button @click="toggleLogin()">Toggle login to on or off</button>
    <div class="buttons" v-if="!isLogin">
      <LoginButtons />
    </div>
    <div class="buttons" v-else>
      <MyDashboardLinks />
    </div>
  </main>
</template>

<style scoped>
main {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 5em 0;
}

main h1 {
  font-size: 2.5em;
  margin-bottom: 1em;
}
.buttons {
  display: flex;
  justify-content: space-around;
  padding: 3em 0;
}
</style>
