<template>
    <a :href="href" target="_blank"><i class='bx' :class="class" ></i></a>
</template>

<script setup lang="ts">
    const props = defineProps({
        class: {
            type: String,
            required: true
        },
        href: {
            type: String,
            required: true
        },
    })
</script>