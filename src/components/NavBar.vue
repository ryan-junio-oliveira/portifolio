<template>
    <nav class="flex items-center justify-between p-6 bg-gray-900 text-white">
        <div class="text-xl font-bold flex items-center justify-center gap-2">
            <i class="fa-solid fa-terminal text-orange-500"></i>
            <h1>Ryan Junio Oliveira</h1>
        </div>
        <a href="#contact" @click.prevent="scrollToContact" class="bg-orange-500 border border-gray-900 py-2 px-4 rounded hover:bg-orange-600 transition cursor-pointer">
            Contact
        </a>
    </nav>
</template>

<script>
export default {
    name: 'NavBar',
    methods: {
        scrollToContact() {
            const contactSection = document.getElementById('contact');
            if (contactSection) {
                contactSection.scrollIntoView({ behavior: 'smooth' });
            }
        }
    }
}
</script>