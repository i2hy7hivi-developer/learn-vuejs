<script setup>

import { ref } from 'vue'

const error = ref('')
const newProject = ref('')
const projects = ref(['MyRentalSpot', 'Rentler', 'Imove360']);

function addProject () {
    
    if (! newProject.value.trim()) {
        error.value = 'Project name is required'
        return
    }

    if (newProject.value.trim()) {
        projects.value.push(newProject.value)
    }
    
    error.value = ''
    newProject.value = ''
}

</script>

<template>
    <div>
        <h4>Projects</h4>
        <ul>
            <li v-for="(project, index) in projects" :key="index">{{ project }}</li>
        </ul>

        <p v-if="error" style="color: red;">{{ error }}</p>

        <input v-model="newProject" placeholder="Enter New Project" />
        <button @click="addProject">Add</button>
    </div>
</template>