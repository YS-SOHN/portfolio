<template>
  <div>
    <swiper :scrollbar="{hide: true,}" :modules="Modules" class="mySwiper" :autoplay="true && {delay:4000}" :loop="true" :navigation="{prevEl: '.swiper-button-prev',nextEl:'.swiper-button-next'}" :pagination="{type:'fraction'}" @slideChange="onSlideChange">
  
    <swiper-slide v-for="(e,index) in 5" :key="index" class="relative">
        <img :src="require(`@/assets/images/burger_${index+1}.png`)" alt="e">
        <div class="absolute left-2/4 top-2/4 -translate-x-2/4 -translate-y-2/4 font-extrabold">
          <h3 data-wow-duration="1s" class="wow animate__fadeInDown text-green-500 text-3xl mice bg-white rounded-xl">{{ TitleData[0][index] }}</h3>
          <h3 data-wow-duration="4s" class="wow animate__fadeIn text-green-500 text-3xl mice bg-white rounded-xl">{{ TitleData[1][0] }}</h3>
        </div>
      </swiper-slide>
    </swiper>
  </div>
</template>

<script>
import {Swiper,SwiperSlide } from 'swiper/vue'
import {Navigation, EffectFade,Autoplay,Pagination} from 'swiper'

import 'swiper/css'
import 'swiper/css/bundle'
import 'swiper/css/pagination'
import 'swiper/css/navigation'

import WOW from 'wowjs';
import 'animate.css'

import Data from '@/assets/Data.json'
  export default {
    name:"HomePage1",
    data() {
      return {
        Modules :[Navigation,EffectFade,Pagination,Autoplay],
        TitleData : Data.title
      }
    },
    components :{
      Swiper,
      SwiperSlide
    },
    mounted(){
      new WOW.WOW({
        boxClass:"wow",
        animateClass:"animate__animated",
        live:false,
        mobile:true
      }).init();
    },
    methods :{
      onSlideChange(){
        new WOW.WOW({
          live:false
        }).init()
      }
    }

  }
</script>

<style lang="scss" scoped>

</style>