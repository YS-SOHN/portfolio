<template>
  <div>
<div class="relative">
  <img :src="'background.jpg'" alt="" class="scale-110">

  <!-- 빨간 짝대기 -->
  <div class="absolute w-50 left-[300px] top-[180px] border-4 h-96 border-red-500 text-red-500 wow animate__fadeInDown">
  </div>

  <div class="absolute left-[300px] bottom-96">
    <h3 data-wow-duration="1s" class="wow animate__fadeInDown text-white md:text-4xl mice rounded-xl cafe24 text-[28px]">
    {{ TitleData[0][2] }}</h3>
    <h3 data-wow-duration="4s" class="wow animate__fadeIn text-white md:text-5xl mice rounded-xl mt-5 cafe24 text-[28px] font-extrabold">저는 프론트엔드 개발자 <span class="text-[#2f6075] font-extrabold">손유상</span> 입니다</h3>
  </div>
</div>
    



    <!-- <swiper :scrollbar="{hide: false}" :modules="Modules" class="mySwiper" :autoplay="true && {delay:5000}" :loop="true" :navigation="true" :pagination="true" @slideChange="onSlideChange">
  
    <swiper-slide v-for="(e,index) in 5" :key="index" class="relative">
        <img :src="require(`@/assets/images/burger_${index+1}.png`)" alt="e">
        <div class="absolute left-2/4 top-2/4 -translate-x-2/4 -translate-y-2/4 font-extrabold">
          <h3 data-wow-duration="1s" class="wow animate__fadeInDown text-white md:text-5xl mice rounded-xl cafe24 text-[28px]">{{ TitleData[0][index] }}</h3>
          <h3 data-wow-duration="4s" class="wow animate__fadeIn text-white md:text-5xl mice rounded-xl mt-5 cafe24 text-[28px]">{{ TitleData[1][0] }}</h3>
        </div>
      </swiper-slide>
    </swiper> -->
  </div>
</template>

<script>


// import 'swiper/css'
// import 'swiper/css/bundle'
// import 'swiper/css/pagination'
// import 'swiper/css/navigation'

import WOW from 'wowjs';
import 'animate.css'

import Data from '@/assets/Data.json'
  export default {
    name:"HomePage1",
    data() {
      return {
        // Modules :[Navigation,EffectFade,Pagination,Autoplay],
        TitleData : Data.title
      }
    },
    // components :{
    //   Swiper,
    //   SwiperSlide
    // },
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

<style>
:root{
  --swiper-theme-color: orange;
}
.swiper-horizontal>.swiper-pagination-bullets, .swiper-pagination-bullets.swiper-pagination-horizontal, .swiper-pagination-custom, .swiper-pagination-fraction{
  width: 90%;
  top: 50%;
  transform: translateY(-50%);
  display: flex;
  flex-direction: column;
  align-items: flex-end;
}
</style>