<script setup>
import { ref } from 'vue'
const username = ref('')
</script>

<template>
  <div>
    <h1>Welcome!</h1>
    <input v-model="username" placeholder="Your name" />
    <p v-if="username">Hello, {{ username }}!</p>
  </div>
</template>
