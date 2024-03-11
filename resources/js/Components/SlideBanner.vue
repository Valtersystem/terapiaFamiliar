<script setup>
import { Swiper, SwiperSlide } from 'swiper/vue';
import { Autoplay, Pagination, Navigation } from 'swiper/modules';

const photos = [
  "https://res.cloudinary.com/dtf70ty3b/image/upload/v1710109103/terapia/1.jpg",
  "https://res.cloudinary.com/dtf70ty3b/image/upload/v1710109103/terapia/2.jpg",
  "https://res.cloudinary.com/dtf70ty3b/image/upload/v1710109103/terapia/3.jpg",
  "https://res.cloudinary.com/dtf70ty3b/image/upload/v1710109103/terapia/4.jpg",
  "https://res.cloudinary.com/dtf70ty3b/image/upload/v1710109103/terapia/5.jpg"
];
</script>

<template>
  <div class="">
    <Swiper
      :modules="[Autoplay, Pagination, Navigation,]"
      :slidesPerView="1"
      :spaceBetween="0"
      :navigation="true"
      :autoplay="true"
      :autoplayOptions ="{delay: 100}"
      :loop="true"
    >
      <SwiperSlide v-for="(photo, index) in photos" :key="index">
        <img :src="photo" alt="">
      </SwiperSlide>
    </Swiper>
  </div>
</template>
