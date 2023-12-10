<script setup>
import axios from 'axios'
import { RouterLink } from 'vue-router'

const apiResp = await fetch('/sensitive-information.json')
const api = await apiResp.json()

const options = {
  method: 'GET',
  url: 'https://api.spoonacular.com/recipes/complexSearch',
  params: {
    number: '20',
    query: 'soup'
  },
  headers: {
    'x-api-key': api.myCookingKey,
    'Content-Type': 'application/json'
  }
}
const response = await axios.request(options)
console.log(response)
</script>

<template>
  <section>
    <v-container>
      <h2 class="mb-4">Recommended Soups</h2>
      <v-row>
        <v-col cols="4" v-for="recipe in response.data.results.slice(3, 6)">
          <router-link :to="{ name: 'RecipeDetail', params: { recipeId: parseInt(recipe.id) } }">
            <v-card height="100%">
              <v-img class="w-100 h-auto" :src="recipe.image"></v-img>
            </v-card>
          </router-link>
          <p class="text-center">{{ recipe.title }}</p>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<style scoped></style>
