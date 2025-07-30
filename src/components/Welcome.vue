<template>
    <h1>Welcome To Vue JS</h1>
    <h2>Hello, {{ username }} 👋</h2>
</template>

<script setup>
defineProps({
  username: String
})
</script>
