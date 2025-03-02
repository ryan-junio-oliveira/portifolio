<template>
    <nav class="flex items-center justify-between p-6 bg-gray-900 text-white">
        <div class="text-xl font-bold">Ryan Junio Oliveira</div>
        <a href="#contact" @click.prevent="scrollToContact" class="border border-white py-2 px-4 rounded hover:bg-gray-800 transition cursor-pointer">
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