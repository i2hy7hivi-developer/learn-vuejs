<script setup>
import { ref } from 'vue'

const show = ref(true);
const projects = ref(['MyRentalSpot', 'Rentler', 'Imove360']);

</script>

<template>
    <h1>Projects List</h1>

    <button @click="show = !show">
        {{ show ? 'Hide Projects' : 'Show Projects' }}
    </button>

    <ul v-if="show">
        <li v-for="(project, i) in projects" :key="i">{{ project }}</li>
    </ul>
</template>