<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HeaderNavVue from './components/HeaderNav.vue';
</script>

<template>
  <v-app>
    <HeaderNavVue />
    <v-main><RouterView /></v-main>
  </v-app>
</template>

<style scoped></style>
