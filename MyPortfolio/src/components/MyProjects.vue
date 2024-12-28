<script setup>
    import {ref} from 'vue';
    import PorjectSingle from './PorjectSingle.vue';

    let projects = ref([
    {
        "name": "E-Commerce API",
        "image": "nodejs.jpg",
        "tags": "Node.js;Express.js;MongoDB",
        "description": "Developed a robust API for an e-commerce platform, including user authentication, product management, and order processing.",
        "task": "Implemented RESTful API endpoints; optimized database queries; integrated third-party payment gateways."
    },
    {
        "name": "Social Media Analytics",
        "image": "python.jpg",
        "tags": "Python;Django;PostgreSQL",
        "description": "Built a platform for analyzing social media trends and sentiment using backend services.",
        "task": "Designed and implemented scalable data pipelines; developed custom APIs for real-time analytics; ensured robust database performance."
    },
    {
        "name": "Real-Time Chat Application",
        "image": "ruby.png",
        "tags": "Ruby;Ruby on Rails;Redis",
        "description": "Created a real-time chat application with features like message storage, read receipts, and typing indicators.",
        "task": "Leveraged WebSocket technology; ensured low-latency communication; implemented robust user authentication."
    },
    {
        "name": "Financial Dashboard",
        "image": "java.png",
        "tags": "Java;Spring Boot;MySQL",
        "description": "Developed a financial dashboard for tracking investments and visualizing portfolio performance.",
        "task": "Integrated multiple third-party APIs for market data; created secure authentication systems; designed the relational database schema."
    },
    {
        "name": "IoT Device Manager",
        "image": "php.jpg",
        "tags": "PHP;Laravel;MariaDB",
        "description": "Engineered a backend for managing IoT devices, including firmware updates and data monitoring.",
        "task": "Implemented secure device communication protocols; developed a user-friendly admin dashboard; ensured high availability."
    },
    {
        "name": "Video Streaming Platform",
        "image": "go.jpeg",
        "tags": "Go;Gin;SQLite",
        "description": "Built the backend for a video streaming platform, enabling seamless video uploads and playback.",
        "task": "Implemented CDN integration; optimized video encoding workflows; ensured high system performance under load."
    }
]);


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