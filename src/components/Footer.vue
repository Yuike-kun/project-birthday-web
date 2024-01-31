<script setup>
const curr = new Date()
</script>

<template>
    <footer class="w-full min-h-12 bg-neutral-900 text-neutral-50 py-4 px-10">
        Copyright <a href="https://github.com/Yuike-kun" class="text-cyan-500">Yuike-kun</a>
        &copy;
        2024 - {{ curr.getFullYear() }}
    </footer>
</template>