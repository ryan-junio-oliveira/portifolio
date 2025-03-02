<template>
    <section id="roadmap" class="bg-gray-100 py-16">
        <div class="max-w-7xl mx-auto text-center py-12 flex flex-col gap-6">
            <h2 class="text-3xl sm:text-4xl font-bold text-gray-900 mb-10 animate-fade-in code-font">LEARNING ROADMAP</h2>

            <p class="text-lg sm:text-xl text-gray-600 mb-8 animate-fade-in-delay">
                Here's a roadmap of my learning journey focusing on essential areas to enhance my skills and become a more complete developer.
            </p>

            <!-- Roadmap Content -->
            <div class="flex flex-col gap-8">
                <!-- Docker & Containerization -->
                <div class="bg-gray-800 text-white p-6 rounded-lg shadow-md animate-fade-in flex items-center gap-4">
                    <div>
                        <h3 class="text-2xl font-bold mb-4 text-orange-500">Docker & Containerization</h3>
                        <i class="fas fa-boxes-stacked fa-2x text-orange-500"></i>
                        <p class="text-gray-400">Learning Docker to create isolated, consistent environments for applications. Understanding container orchestration tools like Kubernetes to efficiently manage containers in production.</p>
                    </div>
                </div>

                <!-- DevOps Practices -->
                <div class="bg-gray-800 text-white p-6 rounded-lg shadow-md animate-fade-in-delay flex items-center gap-4">
                    <div>
                        <h3 class="text-2xl font-bold mb-4 text-orange-500">DevOps & CI/CD Pipelines</h3>
                        <i class="fas fa-tools fa-2x text-orange-500"></i>
                        <p class="text-gray-400">Improving development efficiency through DevOps principles, including automation of testing, deployment pipelines (CI/CD), infrastructure as code, and continuous integration workflows.</p>
                    </div>
                </div>

                <!-- Cloud & Infrastructure -->
                <div class="bg-gray-800 text-white p-6 rounded-lg shadow-md animate-fade-in-delay flex items-center gap-4">
                    <div>
                        <h3 class="text-2xl font-bold mb-4 text-orange-500">Cloud Computing</h3>
                        <i class="fas fa-cloud fa-2x text-orange-500"></i>
                        <p class="text-gray-400">Mastering cloud infrastructure, deployment strategies, and scaling applications using services like AWS and GCP. Focusing on infrastructure security and cost-efficient solutions in the cloud.</p>
                    </div>
                </div>

                <!-- Security & Prevention -->
                <div class="bg-gray-800 text-white p-6 rounded-lg shadow-md animate-fade-in-delay flex items-center gap-4">
                    <div>
                        <h3 class="text-2xl font-bold mb-4 text-orange-500">Web Security & Ethical Hacking</h3>
                        <i class="fas fa-shield-alt fa-2x text-orange-500"></i>
                        <p class="text-gray-400">Building secure web applications by learning security best practices (XSS, CSRF, SQL Injection). Staying ahead of crackers with penetration testing and preventive security strategies.</p>
                    </div>
                </div>

                <!-- Forensics & Investigation -->
                <div class="bg-gray-800 text-white p-6 rounded-lg shadow-md animate-fade-in-delay flex items-center gap-4">
                    <div>
                        <h3 class="text-2xl font-bold mb-4 text-orange-500">Digital Forensics</h3>
                        <i class="fas fa-search fa-2x text-orange-500"></i>
                        <p class="text-gray-400">Exploring digital forensics, analyzing and preserving digital evidence, understanding how to investigate system intrusions, and maintaining data integrity in forensic processes.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'RoadmapSection'
}
</script>
