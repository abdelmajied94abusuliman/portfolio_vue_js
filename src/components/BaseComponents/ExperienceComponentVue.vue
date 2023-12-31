<template>
        <div class="content">
            <div class="year"><i class='bx bxs-calendar'></i>{{ yearFrom }} - {{ yearTo }}</div>
            <h3>{{ title }}</h3>
            <p v-if="description">{{ description }}</p>
            <ul v-if="tasks">
                <li v-for="task in tasks">{{ task }}</li>
            </ul>
        </div>
</template>

<script setup lang="ts">
const props = defineProps({
    yearFrom: {
        type: String,
        required: true,
    },
    yearTo: {
        type: String,
        required: true,
    },
    title: {
        type: String,
        required: true,
    },
    description: {
        type: String,
        required: true,
    },
    tasks: {
        type: Array,
        required: true,
    }
})
</script>