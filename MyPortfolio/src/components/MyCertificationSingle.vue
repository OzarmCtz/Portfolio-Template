<script setup>

const props = defineProps({
        certif: {
            type: Object,
            required : true
        }
    });


</script>

<template>
        <div class="certification">
                <img :src="`/src/assets/certification/${certif.img}`" alt="certification picture">
                <h3 class="text-highlight-1">{{certif.name}}</h3>
                <p class="text-highlight-3">{{ certif.description }}</p>
                <a class="link" :href="`${certif.link}`">View</a>
            </div>
</template>

<style scoped>
    .link:hover {
        color: var(--vt-c-custom-text-2);
    }

.certification img {
        width: 100%;
    }

    .certification h3 {
        font-size: 20px;
        font-weight: bold;
    }

    .certification p {
        font-size: 17px;
        text-align: justify;
    }

    .certification a {
        color: white;
        text-decoration: underline;
        text-underline-offset: 4px ;
    }



</style>