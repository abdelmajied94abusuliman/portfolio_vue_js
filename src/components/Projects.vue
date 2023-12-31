<template>
    <section class="projects" id="projects">
        <h2 class="heading">
            My <span>Projects</span>
        </h2>
        <div class="projects-row">
                <div class="projects-box" v-for="project in ProjectsData">
                    <ProjectComponentVue 
                        :img="project.image"
                        :name-of-project="project.name"
                        :img-alternative="project.altImg"
                        :date="project.date"
                        :description="project.description"
                        :github="project.github"
                    />
                </div>
            </div>
    </section>
</template>

<script setup lang="ts">
    import { ProjectsData } from '@/data/ProjectsData';
    import ProjectComponentVue from './BaseComponents/ProjectComponentVue.vue';
</script>