<script setup></script>

<template>
  <section>
    <!-- <v-row no-gutters>
        <v-col cols="6">
          <h2 class="mb-1">Get your ideas BOILING!</h2>
          <p class="mb-4">Check out our healthiest, and latest recipes in boilingpot.NET!</p>
          <v-btn color="green">
            Recipes
            <v-icon>mdi-arrow-right</v-icon>
          </v-btn>
        </v-col>
      </v-row> -->
    <div class="image-container">
      <v-img class="hero-image" src="/heroimage.webp"></v-img>
      <div class="hero-content w-100">
        <v-container>
          <v-row class="mx-3 align-center justify-center" no-gutters>
            <v-col cols="6">
              <h2>Get your ideas BOILING!</h2>
              <p>Check out the healthiest and most popular recipes here in boilingpot.NET!</p>
            </v-col>
            <v-col class="text-center" cols="6">
              <h3 class="mb-16">
                <v-icon color="green">mdi-circle-medium</v-icon>
                Over 1 MILLION Recipes!
              </h3>
              <v-btn color="green">
                See recipes
                <v-icon>mdi-arrow-right</v-icon>
              </v-btn>
            </v-col>
          </v-row>
        </v-container>
      </div>
    </div>
  </section>
</template>

<style scoped>
.image-container {
  position: relative;
  background-color: black;
}
.hero-image {
  position: relative;
  opacity: 0.45;
}
.hero-content {
  color: white;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
</style>
