<template>
    <section class="home show-animate" id="home">
        <div class="home-content">
            <h1>Hi, I'm <span>Abdelmajied Abu Suliman <span class="animate" style="--i=2"></span></span></h1>
            <div class="text-animate">
                <h3>Full-Stack Developer</h3>
                <span class="animate" style="--i=3"></span>
            </div>
            <p>Junior Full-Stack Developer passionate about crafting meaningful digital solutions. Eager to learn and contribute, I bring enthusiasm, a solid foundation in modern tech, and a commitment to delivering quality work. Let's team up for innovative projects!
                <span class="animate" style="--i=4"></span></p>
            <div class="btn-box">
                <BtnVue
                    class="btn"
                    name-of-button="Hire Me"
                    href="#aboutMe"
                    target=""
                />
                <BtnVue
                    class="btn"
                    name-of-button="Let's Talk"
                    href="#footer"
                    target=""
                />
                <span class="animate" style="--i=5"></span>
            </div>
            <div class="home-social">
                <BtnSocial class="bxl-whatsapp" href="https://wa.me/00962797193116" />
                <BtnSocial class="bxl-gmail" href="mailto:abdelmajied_a@yahoo.com?subject=Request%20Contact&body=Hello%20Mr%20Abu%20Suliman%2C%0A%0AI%20hope%20this%20email%20finds%20you%20well.%0A%0A%3C--%20Write%20Your%20MSG%20--%3E%0A%0ABest%20Regards%0A%3C--%20Your%20Name%20--%3E" />
                <BtnSocial class="bxl-linkedin" href="https://jo.linkedin.com/in/abdelmajied-akram-091567297" />
                <BtnSocial class="bxl-github" href="https://github.com/abdelmajied94abusuliman" />
                <span class="animate" style="--i=6"></span>
            </div>
            <div class="home-imgHover"><span class="animate" style="--i=7"></span></div>
        </div>
    </section>
</template>

<script setup lang="ts">
    import BtnSocial from './BaseComponents/BtnSocial.vue';
    import BtnVue from './BaseComponents/BtnVue.vue'
</script>