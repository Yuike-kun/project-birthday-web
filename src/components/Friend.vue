<script setup>
import Card from './Card.vue'
import 'vue3-carousel/dist/carousel.css'
import { Carousel, Slide, Pagination, Navigation } from 'vue3-carousel'
import FrenData from '@/assets/data/friendsData.json'
</script>

<template>
    <section class="w-full text-center me-auto flex flex-col gap-2 lg:gap-5">
        <span class="text-4xl font-bold flex justify-center bg-slate-400 bg-opacity-30 py-2 m-4 rounded-lg">
            What's Our Friend Say?
        </span>
        <carousel :autoplay="5000" :wrap-around="true">
            <slide v-for="item in FrenData" :key="item" class="gap-10">
                <div class="carousel__item rounded-md bg-slate-200 w-full h-72 bg-opacity-30 transition-all duration-300">
                    <span class="font-semibold text-2xl">
                        {{ item.name }}
                    </span>
                    <img :src="'/src/assets/images/' + item.image" class="rounded-full w-28 h-28 object-cover">
                    <p>
                        {{ item.quote }}
                    </p>
                </div>
            </slide>

            <template #addons>
                <navigation />
                <pagination />
            </template>
        </carousel>
    </section>
</template>

<style scoped>
.carousel__item {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    padding: 4rem;
    gap: 10px
}
</style>