<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <RouterView />
</template>

<style>
html {
  height: 100%;
}

body {
  font-family: 'Outfit', sans-serif;
  min-height: 100vh;
  user-select: none;
}
body::-webkit-scrollbar{
  background-color: transparent;
  width: 4px;
}
body::-webkit-scrollbar-track{
  background-color: transparent;
  width: 4px;
}
body::-webkit-scrollbar-thumb{
  background-color: black;
  width: 4px;
}
</style>
