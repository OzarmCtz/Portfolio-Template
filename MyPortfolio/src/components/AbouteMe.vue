<script setup>
 

</script>

<template>
    <div id="about-me">
        <h2 class="text-highlight-1 section-title">Who am I?</h2>
        <p class="default-text text-highlight-3">
            I am a <span class="text-highlight-2">Backend Developer</span> dedicated to building efficient and scalable systems. 
            With a focus on <span class="text-highlight-2">server-side architecture</span>, I design and implement solutions that ensure reliability and performance.
        </p>
        <p class="default-text text-highlight-3">
            My expertise includes creating <span class="text-highlight-2">RESTful APIs</span> and <span class="text-highlight-2">GraphQL services</span>, 
            optimizing <span class="text-highlight-2">database queries</span>, and enhancing system security. I believe in clean, maintainable code and 
            adhere to <span class="text-highlight-2">best practices</span> in every project.
        </p>
        <p class="default-text text-highlight-3">
            Beyond development, I collaborate closely with cross-functional teams to understand business needs and translate them into 
            <span class="text-highlight-2">technical solutions</span>. Whether it’s building from scratch or improving existing systems, 
            I strive to deliver results that align with both technical and strategic goals.
        </p>
        <br/>
        <p class="default-text text-highlight-2">
            <RouterLink to="/contact" class="custom-link">Contact me !</RouterLink>
        </p>
    </div>
</template>



<style scoped>
    .custom-link {
        display: inline-block;
        padding: 16px 32px;
        background-color: #202837;
        color: white;
        text-align: center;
        text-decoration: none;
        border-radius: 3px;
        font-size: 16px;
        font-weight: bold;
        transition: background-color 0.3s ease, transform 0.2s ease; 
    }

    .custom-link:visited {
        color: white;
    }

    .custom-link:hover {
        background-color: #3a4353;
        transform: scale(1.05);
    }

    .custom-link:active {
        transform: scale(0.98);
    }

    #about-me {
        margin-top: 80px;
    }

    .default-text{
        text-align: justify;
    }

    .default-text span {
        font-weight: bold;
    }
</style>