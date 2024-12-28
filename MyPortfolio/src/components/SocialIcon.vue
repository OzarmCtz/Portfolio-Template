<script setup>
    const props = defineProps({
        img: String,
        link: String,
        alt: String
    })
</script>

<template>
    <a :href="props.link" target="_blank">
        <img class="social-img" :src="`src/assets/aboutme/${props.img}`" :alt="`${props.alt}`">
    </a>
</template>


<style scoped>
     .social-img {
        margin-right: 10px;
        filter: opacity(0.8);
        width: 40px;
    }
</style>