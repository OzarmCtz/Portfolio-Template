<script setup>
    import {ref} from 'vue';
    import PorjectSingle from './PorjectSingle.vue';

    let projects = ref ([
        {
            "name" : "Project n1",
            "image" : "vueproject.png",
            "tags" : "VueJS;PHP;HTML",
            "description" : "ipsum nulla distinctio blanditiis, accusamus excepturi praesentium quisquam veniam, dolorum, debitis velit aperiam perspiciatis.",
            "task" : " In, ipsa sint. Explicabo sunt quaerat a expedita ipsum nulla distinctio blanditiis; accusamus excepturi praesentium quisquam veniam, dolorum, debitis velit aperiam perspiciatis."
        },
        {
            "name" : "Project n2",
            "image" : "vueproject.png",
            "tags" : "VueJS;PHP;HTML",
            "description" : "ipsum nulla distinctio blanditiis, accusamus excepturi praesentium quisquam veniam, dolorum, debitis velit aperiam perspiciatis.",
            "task" : " In, ipsa sint. Explicabo sunt quaerat a expedita ipsum nulla distinctio blanditiis; accusamus excepturi praesentium quisquam veniam, dolorum, debitis velit aperiam perspiciatis."
        },
        {
            "name" : "Project n3",
            "image" : "vueproject.png",
            "tags" : "VueJS;PHP;HTML",
            "description" : "ipsum nulla distinctio blanditiis, accusamus excepturi praesentium quisquam veniam, dolorum, debitis velit aperiam perspiciatis.",
            "task" : " In, ipsa sint. Explicabo sunt quaerat a expedita ipsum nulla distinctio blanditiis; accusamus excepturi praesentium quisquam veniam, dolorum, debitis velit aperiam perspiciatis."
        },
        {
            "name" : "Project n4",
            "image" : "vueproject.png",
            "tags" : "VueJS;PHP;HTML",
            "description" : "ipsum nulla distinctio blanditiis, accusamus excepturi praesentium quisquam veniam, dolorum, debitis velit aperiam perspiciatis.",
            "task" : " In, ipsa sint. Explicabo sunt quaerat a expedita ipsum nulla distinctio blanditiis; accusamus excepturi praesentium quisquam veniam, dolorum, debitis velit aperiam perspiciatis."
        },
        {
            "name" : "Project n5",
            "image" : "vueproject.png",
            "tags" : "VueJS;PHP;HTML",
            "description" : "ipsum nulla distinctio blanditiis, accusamus excepturi praesentium quisquam veniam, dolorum, debitis velit aperiam perspiciatis.",
            "task" : " In, ipsa sint. Explicabo sunt quaerat a expedita ipsum nulla distinctio blanditiis; accusamus excepturi praesentium quisquam veniam, dolorum, debitis velit aperiam perspiciatis."
        },
        {
            "name" : "Project n6",
            "image" : "vueproject.png",
            "tags" : "VueJS;PHP;HTML",
            "description" : "ipsum nulla distinctio blanditiis, accusamus excepturi praesentium quisquam veniam, dolorum, debitis velit aperiam perspiciatis.",
            "task" : " In, ipsa sint. Explicabo sunt quaerat a expedita ipsum nulla distinctio blanditiis; accusamus excepturi praesentium quisquam veniam, dolorum, debitis velit aperiam perspiciatis."
        }
    ])
</script>

<template>
    <div id="projects">
        <h2 class="text-highlight-1 section-title">Some Projects</h2>
        <PorjectSingle v-for="(project , index) in projects" :key="project.name" :project="project" :reverse="index % 2 === 0 ? false : true"/>

    </div>
</template>

<style scoped>
    #projects {
        display: inline-block;
        margin-top: 60px;
    }
</style>