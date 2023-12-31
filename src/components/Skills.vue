<template>
    <section class="skills" id="skills">
        <h2 class="heading">My <span>Skills</span></h2>

        <div class="skills-row">

            <SkillsComponentVue title="Frontend Skills" :skills="FrontEndSkills" />
            <SkillsComponentVue title="Backend Skills" :skills="BackEndSkills" />
            <SkillsComponentVue title="Other Technical Skills" :skills="OtherSkills" />
            
        </div>
    </section>
</template>

<script setup lang="ts">
    import { FrontEndSkills } from '@/data/SkillsData';
    import { BackEndSkills } from '@/data/SkillsData';
    import { OtherSkills } from '@/data/SkillsData';
    import SkillsComponentVue from './BaseComponents/SkillsComponentVue.vue';
</script>