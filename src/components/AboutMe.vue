<template>
    <section id="about-me"
        class="relative bg-gradient-to-b from-gray-900 to-gray-800 text-white py-16 px-8 shadow-lg shadow-gray-900/90">
        <div class="max-w-7xl mx-auto text-center">
            <h2 class="text-3xl sm:text-4xl font-bold mb-6 code-font">
                ABOUT ME
            </h2>
            <p class="text-lg sm:text-xl leading-relaxed max-w-3xl mx-auto mb-8">
                I am a passionate FullStack Developer with over a year of experience in building efficient and scalable web applications.
                I specialize in PHP, Laravel, JavaScript, MySQL, and modern frontend frameworks.
                I love solving complex problems by crafting clean, maintainable, and well-structured code.
                I strive to create user-friendly experiences that solve real-world problems.
            </p>

            <!-- Icons Section -->
            <div class="flex justify-center space-x-8 text-lg">
                <div class="flex flex-col items-center">
                    <i class="fas fa-code text-4xl text-orange-500 mb-2"></i>
                    <p>Web Development</p>
                </div>
                <div class="flex flex-col items-center">
                    <i class="fas fa-server text-4xl text-orange-500 mb-2"></i>
                    <p>Back-end Expertise</p>
                </div>
                <div class="flex flex-col items-center">
                    <i class="fas fa-laptop-code text-4xl text-orange-500 mb-2"></i>
                    <p>Responsive Design</p>
                </div>
                <div class="flex flex-col items-center">
                    <i class="fas fa-project-diagram text-4xl text-orange-500 mb-2"></i>
                    <p>Problem Solving</p>
                </div>
            </div>

            <!-- Call to Action Button -->
            <div class="flex justify-center mt-12">
                <a href="#contact"
                    class="px-6 py-3 bg-orange-500 text-white rounded-lg hover:bg-orange-600 transition-transform transform hover:scale-105 duration-300">
                    Get in Touch
                </a>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'AboutMe'
}
</script>

<style scoped>
i {
    transition: transform 0.3s ease;
}

i:hover {
    transform: scale(1.2);
}
</style>
