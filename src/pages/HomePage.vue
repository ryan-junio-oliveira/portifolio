<template>
    <HeroSection />
    <AbouteMe />
    <SkillsSection />
    <MyProjects />
    <ExperienceSection />
    <RoadmapSection />
    <TicTacToe />
    <ContactSection />

    <!-- Apenas para prencher espaço -->
    <section class="px-2 py-2">
        <div class="max-w-7xl mx-auto text-center py-2 flex flex-col gap-6">
            Apenas para preencher o espaço
        </div>
    </section>

</template>

<script>
import ScrollReveal from "scrollreveal";
import HeroSection from '@components/HeroSection.vue';
import AbouteMe from '@components/AboutMe.vue';
import SkillsSection from '@components/SkillsSection.vue';
import MyProjects from '@components/MyProjects.vue';
import ExperienceSection from '@components/ExperienceSection.vue';
import RoadmapSection from '@components/RoadmapSection.vue';
import ContactSection from '@components/ContactSection.vue';

export default {
    name: 'HomePage',
    components: {
        HeroSection,
        AbouteMe,
        SkillsSection,
        MyProjects,
        ExperienceSection,
        RoadmapSection,
        ContactSection
    },
    mounted() {
        ScrollReveal().reveal('h2', { duration: 1000, origin: 'top', distance: '50px', reset: true });
        ScrollReveal().reveal('p', { duration: 1000, origin: 'bottom', distance: '50px', delay: 200, reset: true });
        ScrollReveal().reveal('a', { duration: 1000, origin: 'bottom', distance: '50px', delay: 400, reset: true });
    }
};
</script>

<style>
#hero-section {
    background: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)), url('/mountains.jpeg');
    height: 100%;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}

@keyframes fade-in {
    0% {
        opacity: 0;
        transform: translateY(20px);
    }

    100% {
        opacity: 1;
        transform: translateY(0);
    }
}

.animate-fade-in {
    animation: fade-in 0.7s ease-out forwards;
}

.animate-fade-in-delay {
    animation: fade-in 0.9s ease-out forwards;
}
</style>
