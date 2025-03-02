<template>
    <!-- Skills Section -->
    <section id="skills" class="bg-gray-100 py-16 mt-6 mb-6">
        <div id="skill-scroll" class="max-w-7xl mx-auto text-center py-12">
            <h2 class="text-3xl sm:text-4xl font-bold text-gray-900 mb-10 animate-fade-in code-font">SKILL & TECHNOLOGIES</h2>
            <p class="text-lg sm:text-xl text-gray-600 mb-8 animate-fade-in-delay">
                A comprehensive stack for developing full-featured web applications.
            </p>
            
            <!-- Skills Grid -->
            <div class="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-4 gap-12 justify-center items-center px-6">
                <!-- Each Skill Item -->
                <div class="group">
                    <img src="/icons/php.svg" alt="PHP" class="h-16 sm:h-20 mx-auto transition-transform duration-300 group-hover:scale-110">
                    <p class="mt-4 text-gray-700 group-hover:text-orange-500 transition-colors">PHP</p>
                </div>

                <div class="group">
                    <img src="/icons/laravel.svg" alt="Laravel" class="h-16 sm:h-20 mx-auto transition-transform duration-300 group-hover:scale-110">
                    <p class="mt-4 text-gray-700 group-hover:text-orange-500 transition-colors">Laravel</p>
                </div>

                <div class="group">
                    <img src="/icons/mysql.svg" alt="MySQL" class="h-16 sm:h-20 mx-auto transition-transform duration-300 group-hover:scale-110">
                    <p class="mt-4 text-gray-700 group-hover:text-orange-500 transition-colors">MySQL</p>
                </div>

                <div class="group">
                    <img src="/icons/javascript.svg" alt="JavaScript" class="h-16 sm:h-20 mx-auto transition-transform duration-300 group-hover:scale-110">
                    <p class="mt-4 text-gray-700 group-hover:text-orange-500 transition-colors">JavaScript</p>
                </div>

                <div class="group">
                    <img src="/icons/git.svg" alt="Git" class="h-16 sm:h-20 mx-auto transition-transform duration-300 group-hover:scale-110">
                    <p class="mt-4 text-gray-700 group-hover:text-orange-500 transition-colors">Git</p>
                </div>

                <div class="group">
                    <img src="/icons/nginx.svg" alt="Nginx" class="h-16 sm:h-20 mx-auto transition-transform duration-300 group-hover:scale-110">
                    <p class="mt-4 text-gray-700 group-hover:text-orange-500 transition-colors">Nginx</p>
                </div>

                <div class="group">
                    <img src="/icons/rabbitmq.svg" alt="RabbitMQ" class="h-16 sm:h-20 mx-auto transition-transform duration-300 group-hover:scale-110">
                    <p class="mt-4 text-gray-700 group-hover:text-orange-500 transition-colors">RabbitMQ</p>
                </div>

                <div class="group">
                    <img src="/icons/linux.svg" alt="Linux" class="h-16 sm:h-20 mx-auto transition-transform duration-300 group-hover:scale-110">
                    <p class="mt-4 text-gray-700 group-hover:text-orange-500 transition-colors">Linux</p>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'SkillsSection'
}
</script>

<style scoped>
.group img {
    transition: transform 0.3s ease;
}

.group:hover img {
    transform: scale(1.2);
}

.group p {
    transition: color 0.3s ease;
}

.group:hover p {
    color: #ff7300; /* orange shade */
}
</style>
