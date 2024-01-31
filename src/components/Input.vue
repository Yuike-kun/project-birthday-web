<script setup>
defineProps({
    label: String,
    name: String,
    type: String
})
</script>

<template>
    <label :for="name">{{ label }}</label>
    <input :type="type" :name="name"
        class="rounded bg-transparent outline-0 border-2 p-1 text-slate-300 transition-all duration-300     ">
</template>