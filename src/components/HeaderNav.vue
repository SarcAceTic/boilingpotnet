<script setup></script>

<template>
  <v-app-bar elevation="1">
    <v-app-bar-nav-icon>
      <v-icon size="40">mdi-pot-steam</v-icon>
    </v-app-bar-nav-icon>
    <v-app-bar-title><h3>boilingpot.NET</h3></v-app-bar-title>
    <v-btn class="w-25 border text-none">
        <template v-slot:prepend>
            <v-icon>mdi-magnify</v-icon>
        </template>
        <p>Search</p>
    </v-btn>
  </v-app-bar>
</template>
