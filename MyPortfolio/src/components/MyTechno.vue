<script setup>
</script> 

<template>
    <div id="skills">
        <h2 class="text-highlight-1 section-title">My Technologies</h2>
        <div id="icons-list">
            <div class="techno-container"><i class="techno-icon devicon-nodejs-plain"></i> <br/> <span>Node.js</span></div>
            <div class="techno-container"><i class="techno-icon devicon-python-plain"></i> <br/> <span>Pyhton</span></div>
            <div class="techno-container"><i class="techno-icon devicon-ruby-plain"></i> <br/> <span>Ruby</span></div>
            <div class="techno-container"><i class="techno-icon devicon-java-plain"></i> <br/> <span>Java</span></div>
            <div class="techno-container"><i class="techno-icon devicon-php-plain"></i> <br/> <span>PHP</span></div>
            <div class="techno-container"><i class="techno-icon devicon-go-original-wordmark"></i> <br/> <span>GO</span></div>
            <div class="techno-container"><i class="techno-icon devicon-angularjs-plain"></i> <br/> <span>AngularJS</span></div>
            <div class="techno-container"><i class="techno-icon devicon-vuejs-plain"></i> <br/> <span>Vue.js</span></div>
            <div class="techno-container"><i class="techno-icon devicon-nuxtjs-plain"></i> <br/> <span>Nuxt.js</span></div>
            <div class="techno-container"><i class="techno-icon devicon-react-original"></i> <br/> <span>React.js</span></div>
            <div class="techno-container"><i class="techno-icon devicon-nextjs-original-wordmark"></i> <br/> <span>Next.js</span></div>
            <div class="techno-container"><i class="techno-icon devicon-symfony-original"></i> <br/> <span>Symfony</span></div>
            <div class="techno-container"><i class="techno-icon devicon-mysql-original"></i> <br/> <span>MySQL</span></div>
            <div class="techno-container"><i class="techno-icon devicon-mongodb-plain"></i> <br/> <span>MongoDB</span></div>
            <div class="techno-container"><i class="techno-icon devicon-git-plain"></i> <br/> <span>Git</span></div>
            <div class="techno-container"><i class="techno-icon devicon-amazonwebservices-plain-wordmark"></i> <br/> <span>AWS</span></div>
        </div>
    </div>
</template>

<style scoped>
    #skills{
        margin-top: 60px;
    }

    #icons-list {
        display: grid;
        grid-template-columns: repeat(8 , 1fr);
        grid-template-rows: repeat(2 , 1fr) ;
        grid-column-gap: 5px ;
        grid-row-gap: 5px;
        margin-top: 35px;
    }

    .techno-container {
        text-align: center;
        color: var(--vt-c-custom-text-1);
        transition: transform 0.5s;
        padding: 10px;
    }

    .techo-container span {
        font-weight: bold;
    }

    .techno-container:hover {
        transform: rotate(15deg) ;
        color: var(--vt-c-custom-text-2);
    }

    .techno-icon {
        font-size: 80px;
        margin: 0 auto;
        color: var(--vt-c-custom-text-1);
    }

    .techno-icon:hover {
        color: var(--vt-c-custom-text-2);
        transform: rotate(15deg);
    }

    @media screen and (max-width: 905px) {
        #icons-list {
            grid-template-columns: repeat(4 , 1fr);
            grid-template-rows: repeat(4 ,1fr);
            grid-column-gap: 5px;
            grid-row-gap: 40px;
        }
    }

    @media screen and (max-width: 450px) {
            #icons-list {
                grid-template-columns: repeat(2 , 1fr);
                grid-template-rows: repeat(8 , 1fr);
                grid-column-gap: 5px;
                grid-row-gap: 20px;
            }
        }

</style>