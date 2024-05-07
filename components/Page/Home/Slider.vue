<script setup>
const sliders = [
  {
    link: 'img/content/slider/banner1.jpg',
  },
  {
    link: 'img/content/slider/banner2.jpg',
  },
  {
    link: 'img/content/slider/banner3.jpg',
  },
]

const sliderInfo = {
  title: `loft <br> мебель`,
  text: 'Современная и удобная мебель в Анапе',
  textBtn: 'СМОТРЕТЬ КАТАЛОГ'
}
</script>

<template>
  <section class="home-slider">
    <div class="container">
      <div class="home-slider__content">
        <Swiper class="home-slider__slider" :modules="[SwiperAutoplay]" :slides-per-view="1" :loop="true" :autoplay="{
          delay: 3000,
          disableOnInteraction: true,
        }">
          <SwiperSlide class="home-slider__slide" v-for="slide in sliders" :key="slide.link"
            :style="{ backgroundImage: `url(${slide.link})` }"></SwiperSlide>
        </Swiper>

        <h1 v-html="sliderInfo.title" class="home-slider__title"></h1>
        <h2 class="home-slider__subtitle">{{ sliderInfo.text }}</h2>
        <NuxtLink to="/catalog" class="home-slider__btn">{{ sliderInfo.textBtn }}</NuxtLink>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.home-slider {
  height: 450px;
  
  &__content {
    position: relative;
    padding-top: 100px;
    padding-left: 120px;
  }

  &__slider {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    width: 100%;
    height: 450px;
    z-index: -1;
  }

  &__slide {
    width: 100%;
    height: 100%;
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
  }

  &__title {
    font-weight: 700;
    font-size: 50px;
    line-height: 105%;
    letter-spacing: 0.02em;
    text-transform: uppercase;
    color: #3c3c3c;
    margin-bottom: 15px;
    background-color: rgba(255, 255, 255, 0.8);
    max-width: fit-content;
    padding: 20px;
    border-radius: 8px;
  }

  &__subtitle {
    font-weight: 400;
    font-size: 16px;
    line-height: 141%;
    letter-spacing: 0.02em;
    color: #343434;
    margin-bottom: 20px;
    background-color: rgba(255, 255, 255, 0.8);
    max-width: fit-content;
    padding: 20px;
    border-radius: 8px;
  }

  &__btn {
    font-weight: 700;
    font-size: 12px;
    line-height: 141%;
    letter-spacing: 0.04em;
    color: #343434;
    padding: 14px 25px;
    box-shadow: 0 2px 4px 0 rgba(0, 0, 0, 0.07);
    background: #fff;
    display: inline-block;
  }
}
</style>
