<template>
  <nav>
    <button @click="$emit('change-page', 'home')">Home</button>
    <button @click="$emit('change-page', 'music')">Music</button>
    <button @click="$emit('change-page', 'games')">Games</button>
  </nav>
</template>
