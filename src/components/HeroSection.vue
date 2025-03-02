<template>
    <section id="hero-section"
        class="box-shadow flex flex-col bg-gray-900 text-white px-12 py-12 shadow-lg shadow-gray-900/90">
        <div class="flex items-center justify-between max-w-7xl mx-auto flex-col md:flex-row p-6 py-24">
            <div>
                <h1 class="text-3xl sm:text-5xl md:text-5xl font-bold leading-tight animate-fade-in code-font">
                    HAY! I'M RYAN <br />
                    <strong class="code-font text-orange-500 font-bold" id="typing-effect"></strong>
                </h1>
                <p class="mt-4 text-lg sm:text-xl text-gray-300 animate-fade-in-delay max-w-4xl">
                    Solve problems by developing solutions, build web applications for 'demanding' users, and seamless
                    web experiences.
                </p>
            </div>
        </div>
    </section>
</template>

<script>
import TypeIt from "typeit";

export default {
    name: "HeroSection",
    mounted() {
        new TypeIt("#typing-effect", {
            strings: ["I'M A DEVELOPER","GRADUATED IN MANAGEMENT", "INFORMATION TECHNOLOGY"],
            speed: 100,
            breakLines: true,
            loop: false,
            deleteSpeed: 50,
            nextStringDelay: [500, 1000],
        }).go();
    },
};
</script>
