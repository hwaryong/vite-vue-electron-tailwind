<script setup>
const powers = [
    { name: 'Vite', url: 'https://vitejs.dev/' },
    { name: 'Vue', url: 'https://vuejs.org/' },
    { name: 'Electron', url: 'https://www.electronjs.org/' },
    { name: 'Tailwind CSS', url: 'https://tailwindcss.com/' },
];
</script>

<template>
    <div class="w-full h-screen flex bg-green-100 text-green-900">
        <div class="m-auto flex gap-8">
            <a
                v-for="power of powers"
                :href="power.url"
                class="text-3xl font-bold"
            >{{ power.name }}</a>
        </div>
    </div>
</template>
