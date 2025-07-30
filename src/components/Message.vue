<script setup>
import { ref } from 'vue'

const isLoggedIn = false;

</script>

<template>
  <div>
    <h2 v-if="isLoggedIn">Welcome back, user! 🎉</h2>
    <h2 v-else>Please log in 🔐</h2>
  </div>
</template>