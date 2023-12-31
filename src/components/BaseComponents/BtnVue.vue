<template>
    <a :href="href" :target="target">
        {{ nameOfButton }}
    </a>
</template>

<script setup lang="ts">
    const props = defineProps({
        nameOfButton: {
            type: String,
            required: true
        },
        href: {
            type: String,
            required: true
        },
        target: {
            type: String,
            required: true
        }
    })
</script>