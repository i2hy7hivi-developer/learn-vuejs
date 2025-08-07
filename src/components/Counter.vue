<script setup>

import { ref } from 'vue'

const count = ref(1)

function decrement () {
    count.value--
}

function increment () {
    count.value++
}
</script>

<template>
    <div>
        <h4>Count: {{ count }}</h4>

        <button @click="increment">+</button>
        <button @click="decrement">-</button>

    </div>
</template>