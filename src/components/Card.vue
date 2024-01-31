<script setup>
defineProps({
    addon: String
})
</script>


<template>
    <div class="p-4 flex flex-col gap-3 mx-4 rounded-md bg-slate-200 bg-opacity-30 transition-all duration-300" :class="addon">
        <slot />
    </div>
</template>