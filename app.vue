<template>
  <div>
    <p class="text-3xl">{{ wordData[0].wordEN }}</p>
    <p class="text-xl">{{ wordData[0].wordCN }}</p>
  </div>
  <div>
    <swiper
      :effect="'cards'"
      :grabCursor="true"
      :modules="modules"
      class="mySwiper"
    >
      <swiper-slide>Slide 1</swiper-slide><swiper-slide>Slide 2</swiper-slide
      ><swiper-slide>Slide 3</swiper-slide><swiper-slide>Slide 4</swiper-slide
      ><swiper-slide>Slide 5</swiper-slide><swiper-slide>Slide 6</swiper-slide
      ><swiper-slide>Slide 7</swiper-slide><swiper-slide>Slide 8</swiper-slide
      ><swiper-slide>Slide 9</swiper-slide>
    </swiper>
  </div>
</template>

<script setup>
import { Swiper, SwiperSlide } from 'swiper/vue';
// Import Swiper styles
import 'swiper/css';
import 'swiper/css/effect-cards';

import '~/assets/css/style.css';
import { EffectCards } from 'swiper';

const modules = [EffectCards];

const wordData = ref([
  {
    wordCN: '年',
    wordEN: 'year',
  },
]);
</script>
