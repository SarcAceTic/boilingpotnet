<script setup>
import HeroSection from '../components/HeroSection.vue';
import RecommendedRecipes from '../components/RecommendedRecipes.vue';
</script>

<template>
  <HeroSection class="mb-4" />
  <Suspense>
    <RecommendedRecipes />
  </Suspense>
</template>

<style scoped>
</style>
