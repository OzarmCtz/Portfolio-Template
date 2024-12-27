<script setup>

    import {ref} from 'vue';
    import MyTutorialSingle from './MyTutorialSingle.vue';


    let tutorial = ref([
        {
            name : "Unity",
            description : "La formation Unity la plus poussé sur le web avec 160h du contenu.",
            link : "https://google.com",
            img : "vueproject.png"
        },
        {
            name : "Unity",
            description : "La formation Unity la plus poussé sur le web avec 160h du contenu.",
            link : "https://google.com",
            img : "vueproject.png"
        },
        {
            name : "Unity",
            description : "La formation Unity la plus poussé sur le web avec 160h du contenu.",
            link : "https://google.com",
            img : "vueproject.png"
        },
        {
            name : "Unity",
            description : "La formation Unity la plus poussé sur le web avec 160h du contenu.",
            link : "https://google.com",
            img : "vueproject.png"
        },
        {
            name : "Unity",
            description : "La formation Unity la plus poussé sur le web avec 160h du contenu.",
            link : "https://google.com",
            img : "vueproject.png"
        },
        {
            name : "Unity",
            description : "La formation Unity la plus poussé sur le web avec 160h du contenu.",
            link : "https://google.com",
            img : "vueproject.png"
        }
    ]);

</script>

<template>
    <div id="tutos">
        <h2 class="text-highlight-1 section-title">Mes formations vidéo</h2>
        <p class="description">Comme expliqué précdemement , j'aime <span class="text-highlight-2">Bla Bla</span></p>
        <div id="formations">
             <MyTutorialSingle 
             v-for="(item , index) in tutorial"
             :key="index"
             :tutorial="item"
             />
            </div>
            <a id="formateur" href="https://google.com" target="_blank">View all formations</a>
    </div>
</template>

<style scoped>
    #tutos {
        margin-top: 60px;
    }

    #tutos .description  {
        text-align: justify;
        font-size: 19px;
    }

    #formations {
        display: grid;
        grid-template-columns: repeat(3 , 1fr);
        grid-template-rows: repeat(2 , 1fr);
        grid-column-gap: 20px;
        grid-row-gap: 50px;
        margin-top: 35px;
    }
    #formateur {
        line-height: 40px;
        color: white;
        text-decoration: underline;
        text-underline-offset: 4px;
        font-size: 20px;
        font-weight: bold;
        display: block;
        width: 100%;
        text-align: center;
        margin-top: 40px;
    }

    @media screen and (max-width: 600px) {
        #formations {
            grid-template-columns: repeat(1, 1fr);
            grid-template-rows: repeat(1 , 1fr);
            grid-column-gap: 0px ;
            grid-row-gap : 20px;
        }
    }
</style>