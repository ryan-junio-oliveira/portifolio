<template>
    <section id="contact" class="bg-gradient-to-br from-orange-600 to-orange-700 text-white px-8 py-16">
        <div class="max-w-7xl mx-auto text-center py-12 flex flex-col gap-6 items-center">
            <!-- Título da Seção -->
            <h2 class="text-4xl sm:text-5xl font-bold mb-6">
                Get in Touch
            </h2>
            
            <!-- Texto de Introdução -->
            <p class="text-lg sm:text-xl mb-8 max-w-2xl">
                I'm always open to discussing new projects, creative ideas, or opportunities to be part of your vision. Whether you need help with development, consultation, or a full project, feel free to reach out.
            </p>
            
            <!-- Botão de Contato -->
            <a href="mailto:ryan.oliveira.personal@outlook.com"
               class="px-8 py-3 bg-white text-orange-600 font-semibold rounded-full hover:bg-gray-100 transition-transform duration-300 hover:scale-105 focus:outline-none focus:ring-4 focus:ring-orange-400 focus:ring-opacity-50 w-64 shadow-lg">
                Contact Me
            </a>

            <!-- Ícones de Redes Sociais -->
            <div class="flex gap-6 mt-8">
                <a href="https://www.linkedin.com/in/ryan-oliveira-717a13235/" target="_blank" aria-label="LinkedIn"
                   class="text-white hover:text-gray-300 transition-transform duration-300 hover:scale-110">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="h-8 w-8" viewBox="0 0 24 24">
                        <path d="M19 0h-14c-2.76 0-5 2.24-5 5v14c0 2.76 2.24 5 5 5h14c2.76 0 5-2.24 5-5v-14c0-2.76-2.24-5-5-5zm-11.52 20.55h-3.07v-11.08h3.07v11.08zm-1.53-12.68h-.02c-1.02 0-1.68-.7-1.68-1.58 0-.9.68-1.58 1.7-1.58s1.68.69 1.68 1.58c0 .89-.66 1.58-1.68 1.58zm12.05 12.68h-3.08v-5.9c0-1.48-.53-2.49-1.87-2.49-1.02 0-1.63.69-1.9 1.36-.1.23-.12.55-.12.87v6.16h-3.08v-11.08h3.08v1.52c.41-.64 1.15-1.56 2.8-1.56 2.04 0 3.57 1.34 3.57 4.22v6.89z"/>
                    </svg>
                </a>
                <a href="https://github.com/ryan-junio-oliveira" target="_blank" aria-label="GitHub"
                   class="text-white hover:text-gray-300 transition-transform duration-300 hover:scale-110">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="h-8 w-8" viewBox="0 0 24 24">
                        <path d="M12 0c-6.63 0-12 5.37-12 12 0 5.31 3.438 9.801 8.205 11.387.6.111.82-.261.82-.579 0-.285-.01-1.041-.015-2.042-3.338.726-4.042-1.611-4.042-1.611-.546-1.387-1.333-1.757-1.333-1.757-1.091-.747.083-.732.083-.732 1.204.084 1.837 1.236 1.837 1.236 1.07 1.834 2.809 1.305 3.495.998.109-.775.418-1.305.761-1.604-2.665-.302-5.466-1.333-5.466-5.931 0-1.31.469-2.381 1.236-3.221-.124-.303-.536-1.521.118-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.292-1.552 3.299-1.23 3.299-1.23.655 1.655.244 2.873.12 3.176.77.84 1.236 1.911 1.236 3.221 0 4.609-2.805 5.625-5.475 5.921.43.371.814 1.102.814 2.222 0 1.606-.014 2.899-.014 3.293 0 .322.216.696.825.578 4.768-1.588 8.205-6.076 8.205-11.386 0-6.63-5.37-12-12-12z"/>
                    </svg>
                </a>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'ContactSection',
}
</script>
