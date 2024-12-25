<script setup>
    import SocialIcon from './SocialIcon.vue';
</script>

<template>
    <div id="top-line">
        <img id="profile-img" src="../assets/me.png" alt="My Picture"> 
        <div id="line">
            <p class="text-highlight-3"><span class="text-highlight-1">OzarmCtz</span>, <br> Développeur d'Applications</p>
            <div id="social">
                <SocialIcon img="github" alt="Github Logo" link="https://github.com/OzarmCtz"/>
                <SocialIcon img="github" alt="Github Logo" link="https://github.com/OzarmCtz"/>
                <SocialIcon img="github" alt="Github Logo" link="https://github.com/OzarmCtz"/>
            </div>
        </div>
    </div>
</template>

<style scoped>
    #profile-img {
    width: 200px;
    height: 200px;
    border-radius: 50%; 
    }

    #top-line{
        margin-top: 50px;
        width: 100%;
        height: 300px;
    }

    #top-line #profile-img {
        float: left;
        margin-right: 50px;
    }

    #top-line #line {
        float: left;
        transform: translateY(40%);
        text-align: center;
    }

    #top-line p {
        font-size: 42px;
        line-height: 60px;
    }

    #top-line p span {
        font-weight: bold;
    }

    #social {
        margin-top: 15px;
    }

    @media screen and (max-width: 905px) {
        #top-line #profile-img {
            display: none;
        }

        #top-line #line {
            float: none ;
            transform: translateY(0%);
        }

        #top-line p {
            font-size: 36px;
        }
    }
    
</style>