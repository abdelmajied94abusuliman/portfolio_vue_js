<template>
    <section id="aboutMe" class="about">
        <h2 class="heading">
            About <span>Me</span>
        </h2>
        <div class="about-img">
            <img src="../assets/images/1667852520649-removebg-preview.png" alt="my-image">
            <span class="circle-spin"></span>
        </div>
        <div class="about-content">
            <h3>Full-Stack Web Developer</h3>
            <p>
                As a Junior Full Stack Developer with a background in Engineering and a Master's degree in Management Engineering, I embody a diverse skill set poised for innovation. Proficient in English and adept in German, I leverage language proficiency to bridge cultures and ideas. Born in 1994, I bring youthful passion and a relentless drive for excellence to every project. Adaptability is my forte; I welcome the opportunity to relocate for career prospects, eager to immerse myself wherever my skills can flourish.
            </p>
            <div class="btn-box btns">
                <BtnVue
                    class="btn"
                    name-of-button="My CV"
                    href="https://drive.google.com/file/d/1wsZUw1viIcOeSw5RHrkOXJaXS6dyxeDK/view?usp=sharing"
                    target="_blank"
                />
            </div>
        </div>

    </section>
</template>

<script setup lang="ts">
    import BtnVue from './BaseComponents/BtnVue.vue';
</script>