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
      Happy Birthday, Dyah Istiqomah
    </span>
    <section class="flex flex-col gap-4">
      <Card addon="hover:bg-opacity-50 max-h-[102rem]">
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-2 place-items-center items-center">
          <div class="col-span-1 overflow-hidden rounded">
            <img src="./assets/images/dyah.jpg" alt="No Image :D"
              class="object-cover rounded hover:scale-110 transition-all duration-300"
              style="width: 25rem; height: 25rem;">
          </div>
          <div class="col-span-2 flex flex-col gap-2 px-5">
            <span class="text-3xl text-center h-12 flex justify-center lg:items-start font-semibold items-center">
              About Dyah
            </span>
            <span class="font-semibold text-justify overflow-auto h-96">
              Meet Dyah, the Grand Duchess of Calm, reigning over the kingdom of Tranquiltopia with a serene smile and a
              whimsical spirit. In the chaotic dance of life, Dyah gracefully pirouettes through challenges, effortlessly
              transforming stress into a lively jigsaw puzzle of possibilities.

              Picture Dyah's tranquil demeanor as a serene lake, reflecting the joy of the world like a mirror. She
              navigates conversations with the finesse of a conversational acrobat, balancing insightful observations with
              the occasional somersault of humor. Her words, carefully chosen and sprinkled with a dash of wit, are like
              the secret ingredients to a laughter potion.

              While Dyah's calm exterior may suggest an air of mystery, beneath the composed facade lies a mischievous
              enchantress. Her laughter, a melodic symphony echoing through the corridors of mirth, is the heartbeat of
              any gathering. Dyah's eyes twinkle with the promise of delightful escapades, leaving friends and
              acquaintances alike eagerly anticipating the next chapter of her whimsical adventures.

              In social settings, Dyah is the guardian of good vibes, weaving an invisible tapestry of positive energy
              that envelops those lucky enough to bask in her radiance. Her reserved nature, rather than a shield, is a
              doorway to an enchanting world of introspection and thoughtful musings. Dyah's presence is a breath of fresh
              air, a zephyr of laughter that sweeps through the mundane and transforms it into a carnival of joy.

              Beyond the tranquil facade, Dyah is a harbinger of happiness, armed with a collection of joyous anecdotes
              and an arsenal of delightful surprises. Her infectious laughter has the magical ability to turn ordinary
              moments into extraordinary memories, and her whimsical charm casts a spell that lingers long after she has
              gracefully departed.

            In the grand tapestry of life, Dyah is the artist, painting strokes of silliness and serenity on a canvas
            that stretches across the horizon of joy. An ambassador of laughter, a sovereign of calm, and an embodiment
            of positivity – Dyah, the one who teaches us that in the grand theater of life, the best roles are played
            with a twinkle in the eye and a hearty laugh as the grand finale.
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