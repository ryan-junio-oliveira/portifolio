<template>
    <section class="bg-gray-900 text-white px-12 py-12">
        <div class="max-w-7xl mx-auto py-12 gap-6 flex flex-col">
            <h2 class="text-3xl font-bold mb-8 text-center animate-fade-in code-font">MY PROJECTS</h2>

            <!-- Repositories Skeleton Loader -->
            <div v-if="isLoading" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="bg-gray-800/50 p-6 rounded-lg shadow-md animate-pulse" v-for="n in 3" :key="n">
                    <div class="h-6 bg-gray-700 w-3/4 mb-4 rounded-md"></div>
                    <div class="h-4 bg-gray-700 w-full mb-2 rounded-md"></div>
                    <div class="h-4 bg-gray-700 w-5/6 rounded-md"></div>
                </div>
            </div>

            <!-- Repositories Content -->
            <div v-if="!isLoading && repositories.length" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div v-for="repo in repositories" :key="repo.id"
                    class="bg-gray-800 p-6 rounded-lg shadow-lg transition-transform duration-500 hover:scale-105 hover:shadow-2xl">
                    <h3 class="text-xl font-bold text-white code-font">{{ repo.name }}</h3>
                    <p class="mt-2 text-gray-400">{{ repo.description || 'No description available' }}</p>
                    <a :href="repo.html_url" target="_blank"
                        class="mt-4 inline-block text-orange-500 hover:underline">View Repository &rarr;</a>
                </div>
            </div>

            <!-- Empty State (No repositories found) -->
            <div v-if="!isLoading && repositories.length === 0" class="text-center text-gray-400">
                <p>No repositories found. Check back later!</p>
            </div>

            <!-- "More" Button -->
            <div class="mt-8 text-center animate-fade-in-delay">
                <a href="https://github.com/ryan-junio-oliveira" target="_blank"
                    class="px-6 py-2 bg-orange-500 hover:bg-orange-600 rounded-lg text-white transition-transform duration-500 hover:scale-105">
                    More Repositories
                </a>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'MyProjects',
    data() {
        return {
            repositories: [],
            isLoading: true,
        };
    },
    async created() {
        setTimeout(() => {
            this.fetchRepositories();
        }, 1500);
    },
    methods: {
        async fetchRepositories() {
            try {
                const response = await fetch('https://api.github.com/users/ryan-junio-oliveira/repos');
                const repos = await response.json();
                this.repositories = repos
                    .sort((a, b) => new Date(b.created_at) - new Date(a.created_at))
                    .slice(0, 6);
            } catch (error) {
                console.error('Failed to fetch repositories:', error);
            } finally {
                this.isLoading = false;
            }
        }
    }
}
</script>
