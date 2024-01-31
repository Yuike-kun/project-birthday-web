<template>
    <nav 
    class="bg-transparent bg-opacity-25 backdrop-blur-sm sticky z-10 top-0 py-4 px-6 transition-all duration-300"
    id="navbar">
        <ul class="flex justify-center gap-5">
            <li v-for="link in links" :key="link" class="font-semibold">
                <a :href="link.to">{{ link.name }}</a>
            </li> 
        </ul>
    </nav>
</template>

<script setup>
import links from '@/assets/data/menu.json'
import { onMounted } from "vue";

const test = () => {
    const nav = document.getElementById('navbar');
    window.onscroll = function () {
        if (document.body.scrollTop >= 200 || document.documentElement.scrollTop >= 200) {
            nav.classList.add("bg-slate-900");
            nav.classList.remove("bg-transparent");
            nav.classList.add("text-neutral-50");
            nav.classList.remove("text-neutral-950");
        }
        else {
            nav.classList.remove("text-neutral-50");
            nav.classList.add("text-neutral-950");
            nav.classList.add("bg-transparent");
            nav.classList.remove("bg-slate-900");
        }
    };
}

onMounted(() => {
    test()
})
</script>