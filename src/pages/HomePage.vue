<template>
    <!-- Hero Section -->
    <section class="flex flex-column bg-gray-900 text-white px-12 py-12">
        <div class="flex items-center justify-between max-w-7xl mx-auto flex-col md:flex-row p-6">
            <div>
                <h1 class="text-4xl sm:text-5xl md:text-6xl font-bold leading-tight animate-fade-in">
                    FullStack Software Web <br />
                    Developer
                </h1>
                <p class="mt-4 text-lg sm:text-xl text-gray-300 animate-fade-in-delay">
                    Solve problems by developing solutions, build web applications for 'demanding' users, and seamless
                    web experiences.
                </p>
                <a href="#about" class="mt-6 inline-block text-purple-500 hover:underline animate-fade-in-delay">
                    About me &rarr;
                </a>
            </div>

            <div class="flex">
                <div class="w-96 h-96 rounded-xl shadow-lg transition-transform duration-500 hover:scale-105">
                    <img src="/svg-home.svg" alt="Developer Illustration" class="animate-fade-in-delay">
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="bg-gray-100 py-16 mt-6 mb-6">
        <div class="max-w-7xl mx-auto text-center py-12 flex flex-col gap-6">
            <h2 class="text-3xl sm:text-4xl font-bold text-gray-900 mb-10 animate-fade-in">Skills & Technologies</h2>
            <p class="text-lg sm:text-xl text-gray-600 mb-8 animate-fade-in-delay">A comprehensive stack for developing
                full-featured web applications.</p>
            <div class="flex flex-wrap gap-8 justify-center items-center px-6">
                <img src="/icons/php.svg" alt="PHP"
                    class="h-16 sm:h-20 hover:scale-110 transition-transform duration-300">
                <img src="/icons/laravel.svg" alt="Laravel"
                    class="h-16 sm:h-20 hover:scale-110 transition-transform duration-300">
                <img src="/icons/mysql.svg" alt="MySQL"
                    class="h-16 sm:h-20 hover:scale-110 transition-transform duration-300">
                <img src="/icons/javascript.svg" alt="JavaScript"
                    class="h-16 sm:h-20 hover:scale-110 transition-transform duration-300">
                <img src="/icons/git.svg" alt="Git"
                    class="h-16 sm:h-20 hover:scale-110 transition-transform duration-300">
                <img src="/icons/nginx.svg" alt="Nginx"
                    class="h-16 sm:h-20 hover:scale-110 transition-transform duration-300">
                <img src="/icons/rabbitmq.svg" alt="RabbitMQ"
                    class="h-16 sm:h-20 hover:scale-110 transition-transform duration-300">
                <img src="/icons/linux.svg" alt="Linux"
                    class="h-16 sm:h-20 hover:scale-110 transition-transform duration-300">
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section class="bg-gray-900 text-white px-12 py-12">
        <div class="max-w-7xl mx-auto py-12 gap-6 flex flex-col">
            <h2 class="text-3xl font-bold mb-8 text-center animate-fade-in">My Projects</h2>

            <!-- Repositories Skeleton Loader -->
            <div v-if="isLoading" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="bg-gray-800/50 p-6 rounded-lg shadow-md animate-pulse" v-for="n in 3" :key="n">
                    <div class="h-6 bg-gray-700 w-3/4 mb-4 rounded-md"></div>
                    <div class="h-4 bg-gray-700 w-full mb-2 rounded-md"></div>
                    <div class="h-4 bg-gray-700 w-5/6 rounded-md"></div>
                </div>
            </div>

            <!-- Repositories Content -->
            <div v-if="!isLoading" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div v-for="repo in repositories" :key="repo.id"
                    class="bg-gray-800 p-6 rounded-lg shadow-md transition-transform duration-500 hover:scale-105">
                    <h3 class="text-xl font-bold text-purple-500">{{ repo.name }}</h3>
                    <p class="mt-2 text-gray-400">{{ repo.description }}</p>
                    <a :href="repo.html_url" class="mt-4 inline-block text-purple-500 hover:underline">View Repository
                        &rarr;</a>
                </div>
            </div>

            <!-- "More" Button -->
            <div class="mt-8 text-center animate-fade-in-delay">
                <a href="https://github.com/ryan-junio-oliveira" target="_blank"
                    class="px-6 py-2 bg-purple-500 hover:bg-purple-600 rounded-lg text-white transition-transform duration-500 hover:scale-105">
                    More Repositories
                </a>
            </div>
        </div>
    </section>

    <!-- Education, Certifications & Professional Experience Section -->
    <section id="experience" class="bg-gray-100 py-16 mt-6 mb-6">
        <div class="max-w-7xl mx-auto text-center py-12 flex flex-col gap-6">
            <h2 class="text-3xl sm:text-4xl font-bold text-gray-900 mb-10 animate-fade-in">Education, Certifications &
                Professional Experience</h2>

            <!-- Education Section -->
            <div class="flex flex-col px-6 text-left items-center">
                <h3 class="text-2xl font-semibold text-gray-900 mb-4 animate-fade-in">Education</h3>
                <div class="bg-gray-800 text-white p-6 rounded-lg shadow-md mb-6 animate-fade-in-delay">
                    <h4 class="text-xl font-bold">Graduated in Information Technology Management</h4>
                    <p class="mt-2 text-gray-400">University of Technology Unifael - Graduated: 2023</p>
                    <p class="mt-2 text-gray-400">Focused on software development, web technologies, IT Process Management and database
                        management.</p>
                </div>
            </div>

            <!-- Certifications Section -->
            <div class="flex flex-col items-start px-6 text-left">
                <h3 class="text-2xl font-semibold text-gray-900 mb-4 animate-fade-in">Certifications</h3>
                <div class="bg-gray-800 text-white p-6 rounded-lg shadow-md mb-6 animate-fade-in-delay">
                    <h4 class="text-xl font-bold">Certified Laravel Developer</h4>
                    <p class="mt-2 text-gray-400">Laravel Certification Program - Issued: 2023</p>
                </div>
                <div class="bg-gray-800 text-white p-6 rounded-lg shadow-md animate-fade-in-delay">
                    <h4 class="text-xl font-bold">AWS Certified Solutions Architect</h4>
                    <p class="mt-2 text-gray-400">Amazon Web Services - Issued: 2024</p>
                </div>
            </div>

            <!-- Professional Experience Section -->
            <div class="flex flex-col items-start px-6 text-left">
                <h3 class="text-2xl font-semibold text-gray-900 mb-4 animate-fade-in">Professional Experience</h3>
                <div class="bg-gray-800 text-white p-6 rounded-lg shadow-md mb-6 animate-fade-in-delay">
                    <h4 class="text-xl font-bold">Software Developer</h4>
                    <p class="mt-2 text-gray-400">XYZ Tech Solutions - Jan 2024 - Present</p>
                    <p class="mt-2 text-gray-400">Developing and maintaining web applications, managing databases, and
                        optimizing backend services using PHP, Laravel, and MySQL.</p>
                </div>
                <div class="bg-gray-800 text-white p-6 rounded-lg shadow-md animate-fade-in-delay">
                    <h4 class="text-xl font-bold">Full-Stack Developer</h4>
                    <p class="mt-2 text-gray-400">ABC Web Solutions - Feb 2022 - Dec 2023</p>
                    <p class="mt-2 text-gray-400">Building scalable web applications and APIs, integrating front-end and
                        back-end solutions, and implementing real-time features with WebSockets.</p>
                </div>
            </div>
        </div>
    </section>


    <!-- Contact CTA Section -->
    <section id="contact" class="bg-gradient-to-br from-purple-600 to-purple-700 text-white px-8 py-16">
        <div class="max-w-7xl mx-auto text-center py-12 flex flex-col gap-6 items-center">
            <h2 class="text-4xl sm:text-5xl font-bold mb-6 animate-fade-in">Get in Touch</h2>
            <p class="text-lg sm:text-xl mb-8 animate-fade-in-delay">I'm always open to discussing new projects,
                creative ideas, or opportunities to be part of your vision.</p>
            <a href="mailto:ryan.oliveira.personal@outlook.com"
                class="px-8 py-3 bg-white text-purple-600 font-semibold rounded-full hover:bg-gray-100 transition-transform duration-300 hover:scale-105 w-64">Contact
                Me</a>
        </div>
    </section>

    <!-- Apenas para prencher espaço -->
    <section class="px-2 py-2">
        <div class="max-w-7xl mx-auto text-center py-2 flex flex-col gap-6">
            Apenas para preencher o espaço
        </div>
    </section>

</template>

<script>
export default {
    name: 'HomePage',
    data() {
        return {
            repositories: [],
            isLoading: true,
        }
    },
    async created() {
        setTimeout(() => {
            this.fetchRepositories();
        }, 2000);
    },
    methods: {
        async fetchRepositories() {
            try {
                const response = await fetch('https://api.github.com/users/ryan-junio-oliveira/repos');
                const repos = await response.json();
                this.repositories = repos
                    .sort((a, b) => new Date(b.created_at) - new Date(a.created_at))
                    .slice(0, 3);
            } catch (error) {
                console.error(error);
            } finally {
                this.isLoading = false;
            }
        }
    }
};
</script>

<style>
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
