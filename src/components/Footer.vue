<script setup>
const curr = new Date()
</script>

<template>
    <footer class="flex justify-end gap-1 w-full min-h-12 bg-neutral-900 text-neutral-50 py-4 px-10">
        <span>
            Copyright <a href="https://github.com/Yuike-kun" class="text-cyan-500">Yuike-kun</a>
            &copy;
            2024 - {{ curr.getFullYear() }}
        </span>
    </footer>
</template>