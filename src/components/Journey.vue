<template>
    <section class="education-experience" id="education-experience">
        <h2 class="heading">
            My <span>Journey</span>
        </h2>
        <div class="education-experience-row">

            <div class="education-experience-column">
                <h3 class="title">
                    Education
                </h3>
                <div class="education-experience-box">
                    <div class="education-experience-content" v-for="education in EducationData">
                        <EducationComponentVue 
                            :year-from="education.yearFrom"
                            :year-to="education.yearTo"
                            :title="education.title"
                            :description="education.description"
                            :name-of-instituation="education.nameOfInstituation"
                            :tasks="education.tasks"
                        />
                    </div>
                </div>
            </div>

            <div class="education-experience-column">
                <h3 class="title">
                    Experience
                </h3>
                <div class="education-experience-box">
                    <div class="education-experience-content" v-for="experience in ExperiencenData">
                        <ExperienceComponentVue 
                            :year-from="experience.yearFrom"
                            :year-to="experience.yearTo"
                            :title="experience.title"
                            :description="experience.description"
                            :tasks="experience.tasks"
                        />
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup lang="ts">
    import EducationComponentVue from './BaseComponents/EducationComponentVue.vue';
    import ExperienceComponentVue from './BaseComponents/ExperienceComponentVue.vue';
    import EducationData from '@/data/EducationData';
    import ExperiencenData from '@/data/ExperienceData';

</script>