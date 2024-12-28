<script setup>
    // Configuration of sections (true = enabled, false = disabled)
    const config = {
        aboutMe: true,        // Enable/Disable the "About Me" section
        techno: true,         // Enable/Disable the "Techno" section
        xp: true,             // Enable/Disable the "Experience" section
        projects: true,       // Enable/Disable the "Projects" section
        certification: true   // Enable/Disable the "Certification" section
    };
    
    // Import components
    import PageTitle from '@/components/PageTitle.vue';
    import AboutMe from '@/components/AbouteMe.vue'; 
    import MyTechno from '@/components/MyTechno.vue';
    import MyXp from '@/components/MyXp.vue';
    import MyProjects from '@/components/MyProjects.vue';
    import MyCertification from '@/components/MyCertification.vue';
</script>


<template>
    <div>
        <PageTitle />

        <!-- "About Me" section conditionally displayed -->
        <AboutMe v-if="config.aboutMe" />
        
        <!-- "Techno" section conditionally displayed -->
        <MyTechno v-if="config.techno" />
        
        <!-- "Experience" section conditionally displayed -->
        <MyXp v-if="config.xp" />
        
        <!-- "Projects" section conditionally displayed -->
        <MyProjects v-if="config.projects" />
        
        <!-- "Certification" section conditionally displayed -->
        <MyCertification v-if="config.certification" />
    </div>
</template>


<style scoped></style>
