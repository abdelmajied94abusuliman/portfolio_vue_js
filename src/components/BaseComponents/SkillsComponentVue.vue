<template>
    <div class="skills-column">
        <div class="title">{{ title }}</div>

        <div class="skills-box">
            <div class="skills-content">

                <div class="progress" v-for="skill in skills">
                    <h3>{{ skill.skill }} <span>{{skill.progress}}%</span></h3>
                    <div class="bar"><span :style="{ width: skill.progress + '%' }" :class="{ 'animate-progress': animate }"></span></div>
                </div>

            </div>
        </div>
    </div>
</template>

<script setup lang="ts">
    import { ref, onMounted } from 'vue';

    const props = defineProps({
        title:{
            type: String,
            required: true,
        },
        skills:{
            type: Object,
            required: true,
        }
    });
    
    const animate = ref(false);

    onMounted(() => {
        animate.value = true;
    });
</script>