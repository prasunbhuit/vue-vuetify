<script setup lang="ts">
  import { computed } from "vue";
  import { destinations } from "../assets/data.json";

  const places = computed(() =>
    destinations.map((el) => ({
      name: el.name,
      slug: el.slug,
    })),
  );
</script>

<template>
  <v-app-bar class="bg-teal">
    <div class="ma-7">
      <h3>Travel Blog</h3>
    </div>
    <router-link v-for="place in places" :key="place.slug" :to="`/${place.slug}`">
      <v-btn>{{ place.name }}</v-btn>
    </router-link>
  </v-app-bar>
</template>

<style scoped></style>
