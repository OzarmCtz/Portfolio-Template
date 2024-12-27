<script setup>

const props = defineProps({
        books: {
            type: Object,
            required : true
        }
    });


</script>

<template>
        <div class="book">
                <img :src="`/src/assets/projects/${books.img}`" alt="book picture">
                <h3 class="text-highlight-1">{{books.name}}</h3>
                <p class="text-highlight-3">{{ books.description }}</p>
                <a :href="`${books.link}`">View</a>
            </div>
</template>

<style scoped>

    .book img {
        width: 100%;
    }

    .book h3 {
        font-size: 20px;
        font-weight: bold;
    }

    .book p {
        font-size: 17px;
        text-align: justify;
    }

    .book a {
        color: white;
        text-decoration: underline;
        text-underline-offset: 4px ;
    }



</style>