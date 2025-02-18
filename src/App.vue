<script setup lang="ts">
  import NavbarView from "./layouts/NavbarView.vue";
</script>

<template>
  <v-layout class="rounded rounded-md">
    <NavbarView />
    <router-view></router-view>
  </v-layout>
</template>

<style scoped></style>
