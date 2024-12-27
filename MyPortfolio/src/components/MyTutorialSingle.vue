<script setup>

const props = defineProps({
        tutorial: {
            type: Object,
            required : true
        }
    });


</script>

<template>
        <div class="formation">
                <img :src="`/src/assets/projects/${tutorial.img}`" alt="formation picture">
                <h3 class="text-highlight-1">{{tutorial.name}}</h3>
                <p class="text-highlight-3">{{ tutorial.description }}</p>
                <a :href="`${tutorial.link}`">View</a>
            </div>
</template>

<style scoped>

.formation img {
        width: 100%;
    }

    .formation h3 {
        font-size: 20px;
        font-weight: bold;
    }

    .formation p {
        font-size: 17px;
        text-align: justify;
    }

    .formation a {
        color: white;
        text-decoration: underline;
        text-underline-offset: 4px ;
    }



</style>