<script setup>
import { onMounted } from "vue";
import Card from './Card.vue'

let theTimer = [
    "days",
    "hour",
    "minute",
    "second"
]

const countdownFunc = () => {
    var countDownDate = new Date("Feb 30, 2024 15:37:25").getTime();

    // Update the count down every 1 second
    var x = setInterval(() => {

        // Get today's date and time
        var now = new Date().getTime();

        // Find the distance between now and the count down date
        var distance = countDownDate - now;

        // Time calculations for days, hours, minutes and seconds
        var days = Math.floor(distance / (1000 * 60 * 60 * 24));
        var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
        var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
        var seconds = Math.floor((distance % (1000 * 60)) / 1000);

        // Display the each result in the element with id's
        document.getElementById("days").innerHTML = days + "d"
        document.getElementById("hour").innerHTML = hours + "h"
        document.getElementById("minute").innerHTML = minutes + "m"
        document.getElementById("second").innerHTML = seconds + "s"

        // If the count down is finished, write some text
        if (distance < 0) {
            clearInterval(x);
            document.getElementById("invitation").innerHTML = "Thanks For Coming :3";
            document.getElementById("days").innerHTML = "0" + "d"
            document.getElementById("hour").innerHTML = "0" + "h"
            document.getElementById("minute").innerHTML = "0" + "m"
            document.getElementById("second").innerHTML = "0" + "s"
        }
    }, 1000);
}

onMounted(() => {
    countdownFunc()
})
</script>

<template>
    <article
        class="flex flex-col gap-5 items-center justify-center from-blue-400 bg-gradient-to-br to-fuchsia-600 p-4 rounded w-full lg:hover:w-2/3 lg:hover:scale-105 transition-all duration-300 text-slate-100"
        id="invite">
        <header class="text-center">
            <span class="text-5xl font-semibold lg:text-7xl" id="invitation">
                We are inviting you
            </span>
        </header>
        <section class="">
            <div class="flex gap-5 bg-slate-200 bg-opacity-30 p-4 rounded">
                <span v-for="item in theTimer" :key="item" :id="item" class="font-semibold text-4xl"></span>
            </div>
        </section>
    </article>
</template>