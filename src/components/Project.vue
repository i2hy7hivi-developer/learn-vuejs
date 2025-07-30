<script setup>
import { ref } from 'vue'

const projects = ['MyRentalSpot', 'Rentler', 'Imove360'];

</script>

<template>
    <h1>Projects List</h1>
    <ul>
        <li
            v-for="(project, index) in projects"
            :key="index">
            {{ project }}
        </li>
    </ul>
</template>