<script setup>

    import {ref} from 'vue';
    import MyCertificationSingle from './MyCertificationSingle.vue';


    let certif = ref([
    {
        name: "AWS Certified Solutions Architect – Associate",
        description: "Demonstrates expertise in designing and deploying scalable systems on AWS.",
        link: "https://aws.amazon.com/certification/certified-solutions-architect-associate/",
        img: "aws.png"
    },
    {
        name: "Docker Certified Associate",
        description: "Validates skills in containerization and Docker ecosystem tools.",
        link: "https://www.docker.com/certification/",
        img: "docker.png"
    },
    {
        name: "Certified Kubernetes Administrator (CKA)",
        description: "Proves proficiency in Kubernetes administration, networking, and storage.",
        link: "https://training.linuxfoundation.org/certification/certified-kubernetes-administrator-cka/",
        img: "kubernetes.jpg"
    },
    {
        name: "Cisco Certified Network Associate (CCNA)",
        description: "Certifies foundational skills in networking, security, and connectivity.",
        link: "https://www.cisco.com/c/en/us/training-events/training-certifications/certifications.html",
        img: "Cisco.jpg"
    },
    {
        name: "Microsoft Certified: Azure Solutions Architect Expert",
        description: "Specializes in designing and implementing solutions on Microsoft Azure.",
        link: "https://learn.microsoft.com/en-us/certifications/azure-solutions-architect/",
        img: "azure.jpeg"
    },
    {
        name: "Google Professional Cloud Architect",
        description: "Demonstrates ability to design cloud solutions on Google Cloud Platform.",
        link: "https://cloud.google.com/certification/cloud-architect",
        img: "google.png"
    }
]);


</script>

<template>
    <div id="certif">
        <h2 class="text-highlight-1 section-title">Certifications</h2>
        <p class="description text-highlight-3">
            I have a passion for continuous learning and love to accumulate 
            <span class="text-highlight-2">professional certifications</span>. 
            Each certification represents a step forward in mastering key technologies and 
            <span class="text-highlight-2">staying updated</span> in the dynamic world of backend development.
        </p>
        <div id="certification">
            <MyCertificationSingle 
                v-for="(item, index) in certif"
                :key="index"
                :certif="item"
            />
        </div>
    </div>
</template>


<style scoped>
    #certif {
        margin-top: 60px;
    }

    #certif .description  {
        text-align: justify;
        font-size: 19px;
    }

    #certification {
        display: grid;
        grid-template-columns: repeat(3 , 1fr);
        grid-template-rows: repeat(2 , 1fr);
        grid-column-gap: 20px;
        grid-row-gap: 50px;
        margin-top: 35px;
    }

    @media screen and (max-width: 600px) {
        #certification {
            grid-template-columns: repeat(1, 1fr);
            grid-template-rows: repeat(1 , 1fr);
            grid-column-gap: 0px ;
            grid-row-gap : 20px;
        }
    }
</style>