<script setup>
    import { ref } from 'vue';

    let activeBloc = ref(0);

    let experiences = ref([
        {
            title : "Développeur Web 1",
            date : "2010 - 2020",
            line1 : "Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet.",
            line2 : "Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet.",
            line3 : "Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet."
        },
        {
            title : "Développeur Web 2 ",
            date : "2010 - 2020",
            line1 : "Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet.",
            line2 : "Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet.",
            line3 : "Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet."
        },
        {
            title : "Développeur Web 3",
            date : "2010 - 2020",
            line1 : "Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet.",
            line2 : "Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet.",
            line3 : "Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet."
        }
    ]);

    const showXp = (id) => {
        activeBloc.value = id;
    }
</script>

<template>
    <div id="xp">
        <h2 class="text-highlight-1 section-title">Expériences</h2>
        <div id="left" class="text-highlight-3">
            <p :class="activeBloc === 0 ? 'active' : '' " class="company fw600" @click="showXp(0)">Sociéte n°1</p>
            <p :class="activeBloc === 1 ? 'active' : '' " class="company fw600" @click="showXp(1)">Sociéte n°2</p>
            <p :class="activeBloc === 2 ? 'active' : '' " class="company fw600" @click="showXp(2)">Sociéte n°3</p>
        </div>
        <div id="right">
            <template v-for="(job,index) in experiences">
                <div class="job-details text-highlight-3" :class="index === activeBloc ? '' : 'hide'" :id="'bloc_' + index">
                    <h3 class="fw600">{{ job.title }}</h3>
                    <span id="date">{{ job.date }}</span>
                    <br/>
                    <p class="fw600 mtb8" style="margin-top: 10px;"><span class="text-highlight-2">X</span>{{ job.line1 }}</p>
                    <p class="fw600 mtb8" style="margin-top: 10px;"><span class="text-highlight-2">X</span>{{ job.line1 }}</p>
                    <p class="fw600 mtb8" style="margin-top: 10px;"><span class="text-highlight-2">X</span>{{ job.line1 }}</p>
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