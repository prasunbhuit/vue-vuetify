<script setup lang="ts"></script>

<template>
  <v-layout class="rounded rounded-md">
    <v-app-bar class="bg-teal">
      <div class="ma-7">
        This is the application bar
      </div>
    </v-app-bar>

    <v-navigation-drawer>
      <v-list>
        <v-list-item title="Navigation drawer"></v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-main
      class="d-flex align-center justify-center bg-teal-lighten-5"
      style="min-height: 100vh"
    >
      Main Content
    </v-main>
  </v-layout>
</template>

<style scoped></style>
