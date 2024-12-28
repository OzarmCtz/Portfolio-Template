<script setup>
    import { ref } from 'vue';

    let activeBloc = ref(0);

    let experiences = ref([
        {
            title: "Backend Developer - TechCorp Solutions",
            date: "2015 - 2020",
            line1: "Designed and implemented RESTful APIs to support scalable web and mobile applications.",
            line2: "Maintained and optimized database systems using PostgreSQL, ensuring data integrity and performance.",
            line3: "Collaborated with front-end developers to integrate user-facing elements with server-side logic."
        },
        {
            title: "Senior Backend Developer - CodeMasters Inc.",
            date: "2020 - 2023",
            line1: "Led a team of developers in building a microservices architecture for a cloud-based SaaS platform.",
            line2: "Implemented advanced authentication and authorization systems using OAuth2 and JWT.",
            line3: "Enhanced application performance by 30% through efficient caching strategies and code optimization."
        },
        {
            title: "Backend Engineer - CloudWare Systems",
            date: "2023 - Present",
            line1: "Architected serverless backend solutions using AWS Lambda and DynamoDB for cost-effective scalability.",
            line2: "Integrated third-party APIs, including payment gateways into enterprise-level systems.",
            line3: "Contributed to DevOps practices, streamlining CI/CD pipelines with Docker and Kubernetes."
        }
    ]);


    const showXp = (id) => {
        activeBloc.value = id;
    }
</script>

<template>
    <div id="xp">
        <h2 class="text-highlight-1 section-title">Experiences</h2>
        <div id="left" class="text-highlight-3">
            <p :class="activeBloc === 0 ? 'active' : '' " class="company fw600" @click="showXp(0)">Company #1</p>
    <p :class="activeBloc === 1 ? 'active' : '' " class="company fw600" @click="showXp(1)">Company #2</p>
    <p :class="activeBloc === 2 ? 'active' : '' " class="company fw600" @click="showXp(2)">Company #3</p>

        </div>
        <div id="right">
            <template v-for="(job,index) in experiences">
                <div class="job-details text-highlight-3" :class="index === activeBloc ? '' : 'hide'" :id="'bloc_' + index">
                    <h3 class="fw600">{{ job.title }}</h3>
                    <span id="date">{{ job.date }}</span>
                    <br/>
                    <p class="fw600 mtb8" style="margin-top: 10px;"><span class="text-highlight-2">-> </span>{{ job.line1 }}</p>
                    <p class="fw600 mtb8" style="margin-top: 10px;"><span class="text-highlight-2">-> </span>{{ job.line2 }}</p>
                    <p class="fw600 mtb8" style="margin-top: 10px;"><span class="text-highlight-2">-> </span>{{ job.line3 }}</p>
                </div>
            </template>
        </div>
    </div>
</template>

<style scoped>

    #xp {
        margin-top: 60px;
    }

    #left  {
        margin-top: 30px;
    }

    #right  {
        margin-top: 30px;
    }


    #xp #left {
        float: left;
        width: 25%;
    }

    #xp #right {
        float: left;
        width: 75%;
    }

    #xp #right {
        float: left;
        width: 75%;
    }

    #xp #right h3 {
        font-size: 20px;
    }

    .fw600 {
        font-weight: 600;
    }

    .mtb8 {
        margin: 8px 0px;
    }

    #date {
        font-style: italic;
        font-size: 14px;
    }

    .company {
        border-left: 4px solid var(--vt-c-custom-text-1) ;
        line-height: 30px;
        padding-left: 10px;
    }

    .active  {
        border-left: 4px solid var(--vt-c-custom-text-2);
        color: var(--vt-c-custom-text-2);
    }

    .company:hover {
        cursor: pointer;
        color: var(--vt-c-custom-text-1);
    }

    .hide {
        display: none ;
    }

    @media screen and (max-width: 600px) {
        #xp #right {
            width: 100%;
            margin-top: 20px;
        }

        #xp #left {
            width: 100%;
        }

        .company {
            border: none;
            padding-left: 0px;
            float:left;
            margin-right: 10px;
        }
    }




</style>