<script setup>
import { ref } from 'vue'
import NavBar from './components/NavBar.vue'
import HomePage from './components/HomePage.vue'
import MusicPage from './components/MusicPage.vue'
import GamesPage from './components/GamesPage.vue'

const currentPage = ref('home')
</script>

<template>
  <NavBar @change-page="currentPage = $event" />
  <HomePage v-if="currentPage === 'home'" />
  <MusicPage v-if="currentPage === 'music'" />
  <GamesPage v-if="currentPage === 'games'" />
</template>
