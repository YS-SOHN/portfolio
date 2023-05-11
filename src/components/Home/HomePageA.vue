<template>
  <div>
    <swiper :scrollbar="{hide: true,}" :modules="Modules" class="mySwiper" :autoplay="true && {delay:2500}" :loop="true" :navigation="{prevEl: '.swiper-button-prev',nextEl:'.swiper-button-next'}" :pagination="{type:'fraction'}" @slideChange="onSlideChange">
  
    <swiper-slide v-for="(e,index) in 5" :key="index" class="relative">
        <img :src="require(`@/assets/images/burger_${index+1}.png`)" alt="e">
        <div class="absolute left-2/4 top-2/4 -translate-x-2/4 -translate-y-2/4 text-orange-500 font-extrabold">
          <h3 data-wow-duration="1s" class="wow animate__fadeInDown">세상에 밝은 빛을 전해줄</h3>
          <h3 data-wow-duration="5s" class="wow animate__fadeIn">저는 프론트엔드 개발자 입니다.</h3>
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
  export default {
    name:"HomePage1",
    data() {
      return {
        Modules :[Navigation,EffectFade,Pagination,Autoplay]
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