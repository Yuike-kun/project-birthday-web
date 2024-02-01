<script setup>
import { onMounted } from 'vue';
import Card from './components/Card.vue';
import Navbar from './components/Navbar.vue';
import Countdown from './components/Countdown.vue';
import Friend from './components/Friend.vue';
import Location from './components/Contact.vue';
import Footer from './components/Footer.vue'
</script>


<template>
  <Navbar />
  <article class="flex flex-col justify-center items-center py-20 gap-20" id="about">
    <span class="sm:text-6xl text-5xl text-center pretty-font" id="home">
      Happy Birthday, Koneko Toujou
    </span>
    <section class="flex flex-col gap-4">
      <Card addon="hover:bg-opacity-50 max-h-[102rem]">
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-2 place-items-center items-center">
          <div class="col-span-1 overflow-hidden rounded">
            <img src="./components/images/konekolovey.jpg" alt="No Image :D"
              class="object-cover rounded hover:scale-110 transition-all duration-300"
              style="width: 25rem; height: 25rem;">
          </div>
          <div class="col-span-2 flex flex-col gap-2 px-5">
            <span class="text-3xl text-center h-12 flex justify-center lg:items-start font-semibold items-center">
              About Koneko
            </span>
            <span class="font-semibold text-justify overflow-auto h-96">
              Koneko Toujou, originally named Shirone is one of the female protagonists of High School DxD. At first, she
              is a first-year student at Kuoh Academy, prior to becoming a second-year, and a member of the Occult
              Research Club. She is a Nekoshou, a rare species of Nekomata, and the younger sister of Kuroka, as well as
              Rias Gremory's first Rook. <br>
              Having become one of Issei's fiancées, then coming to terms with herself, her past, and making amends with
              Kuroka, Koneko started going by Shirone Toujou.Due to witnessing her sister supposedly losing control over her nekomata power and killing her master, Koneko became traumatized by the event, causing her to become withdrawn into herself and stripping her of most of her emotions. As a result, Koneko originally had a quiet and cold personality, rarely showing any feelings or emotions, even when she was speaking. <br>
              It is noted that her serious personality is a result of receiving influence from Rias and is antithetical to her sister's mischievous and outgoing personality. She was also the only one in the group who did not initially get along with Issei, often insulting and rebuking the latter for his perverted nature, although she reveals that she respects him for never giving up and considers him a hard worker. <br>
              Born as Shirone, Koneko is a young Nekomata who is part of a rare species among her kind, called the Nekoshou. She was born from the union between a human father and a Nekomata mother named Fujimai. Her father was a scientist who did not acknowledge Koneko or was aware that she was his child, and merely used her as a subject for his experiments. Her parents eventually died in an experiment-related accident. However, her older sister Kuroka, omitted the truth and any other details about them from Koneko to protect her.
            </span>
          </div>
        </div>
      </Card>
    </section>
    <Countdown />
    <Friend />
    <Location />

</article>
<Footer /></template>