<script setup>
import { ref } from 'vue'

const isLoggedIn = false;

</script>

<template>
  <div>
    <h2 v-show="isLoggedIn">Welcome back, user! 🎉</h2>
  </div>
</template>