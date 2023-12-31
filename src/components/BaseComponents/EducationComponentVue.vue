<template>
    <div class="content">
        <div class="year"><i class='bx bxs-calendar'></i>{{ yearFrom }} - {{ yearTo }}</div>
        <h3>{{ title }}</h3>
        <h2>Institution : {{ nameOfInstituation }}</h2>
        <p>{{ description }}</p>
        <ul>
            <li v-for="task in tasks">
                {{ task }}
            </li>
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
        nameOfInstituation: {
            type: String,
            required: true,
        },
        description: {
            type: String as () => String | undefined,
            required: true,
        },
        tasks: {
            type: Array as () => String[] | undefined,
            required: true,
        },
    })
</script>