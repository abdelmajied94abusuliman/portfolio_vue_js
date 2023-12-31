<template>
    <div class="projects-content">
        <img class="projects-image" :src="img" :alt="imgAlternative">
        <h3 class="title">{{ nameOfProject }} <span class="date">{{ date }}</span></h3>
        <p class="description">{{ description }}</p>
        <div class="home-social-project">
            <a :href="github" class="githubIcon"><i class='bx bxl-github' ></i></a>
        </div>
    </div>
</template>

<script setup lang="ts">
    const props = defineProps({
        img:{
            type: String,
            required: true,
        },
        nameOfProject:{
            type: String,
            required: true,
        },
        date:{
            type: String,
            required: true,
        },
        description:{
            type: String,
            required: true,
        },
        imgAlternative:{
            type: String,
            required: true,
        },
        github:{
            type: String,
            required: true,
        },
    });
</script>