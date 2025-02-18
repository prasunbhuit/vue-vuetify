<script setup lang="ts">
  import { destinations } from "../assets/data.json";
</script>

<template>
  <v-main class="d-flex bg-teal-lighten-5" style="min-height: 100vh; max-width: 100vw">
    <div class="mx-10 my-5">
      <h2>All Destinations</h2>
      <div class="d-flex flex-row flex-wrap">
        <v-col cols="5" v-for="dest in destinations" :key="dest.id">
          <v-card>
            <v-card-item>
              <v-card-title>{{ dest.name }}</v-card-title>
              <v-card-subtitle>{{ dest.slug }}</v-card-subtitle>
              <v-img :src="`/images/${dest.image}`"></v-img>
              <v-card-action>Go To</v-card-action>
            </v-card-item>
          </v-card>
        </v-col>
      </div>
    </div>
  </v-main>
</template>

<style scoped></style>
