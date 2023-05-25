<template>
  <!-- <div class="flex flex-wrap">
    <div v-for="(e,index) in Contents" :key="e" class="flex justify-between">
            <div>
              <img :src="require(`@/assets/images/port_${index}.png`)" alt="img" class="w-[25%]">
               <p>{{ e.title }}</p>
               <p>{{ e.desc }}</p>
               <p>{{ e.desc2 }}</p>
               <p>{{ e.desc3 }}</p>

            </div>
              
            </div>

  </div> -->


  <div>
    <div class="w-full">
      <div class="w-7xl mx-auto">
          <div class="max-w-7xl mx-auto flex justify-center flex-wrap relative">
            <div class="flex flex-wrap gap-x-[2%]">
              <div v-for="(e,index) in Contents" :key="e" class="relative group overflow-hidden  gap-y-5 mb-5 md:w-[48%] lg:w-[32%] w-[99%] sm:mx-auto">
                   <img :src="require(`@/assets/images/port_${index}.png`)" alt="" class="rounded-md hover:opacity-50 group-hover:scale-105 transition-all w-[400px] mx-auto">
                   <div class="mx-auto text-center">
                     <h2 class="font-extrabold mt-3">{{ e.title }}</h2>
                     <p>{{ e.desc }}</p>
                     <p>{{ e.desc2 }}</p>
                     <p>{{ e.desc3 }}</p>
                     <p>{{ e.desc4 }}</p>
                   </div>
                   
                  <button class="absolute group-hover:left-2/4 top-2/4 group-hover:-translate-x-2/4 -translate-y-2/4 text-white group-hover:opacity-100  opacity-0 left-0 transition-all duration-500 border w-28 rounded-2xl bg-orange-500 h-10"><a :href="e.link" target="_blank"> Move into</a></button><br>
                  <button class="absolute mt-12 group-hover:right-2/4 right-0 top-2/4 group-hover:translate-x-2/4 -translate-y-2/4 text-white group-hover:opacity-100 opacity-0 transition-all duration-500 border w-28 rounded-2xl bg-orange-500 h-10">git Hub</button>
                </div>
            </div>
          </div>
      </div>
    </div>
  </div>
</template>

<script>
  // Import Swiper Vue.js components
  // import { Swiper, SwiperSlide } from 'swiper/vue';

  // Import Swiper styles
  import 'swiper/css';

  import 'swiper/css/pagination';
  import 'swiper/css/navigation';

  // import './style.css';

  // import required modules
  // import { Pagination, Navigation } from 'swiper';
  import Data from '@/assets/Data.json'

  export default {
    components: {
      // Swiper,
      // SwiperSlide,
    },
    setup() {
      return {
        // modules: [Pagination, Navigation],
      };
    },
    data() {
      return {
        Contents:Data.contents
      }
    },
  };
</script>

<style>

</style>



  <!-- <div class="bg-yellow-500 h-[970px]">portfolio
          <div class="w-full h-full relative group">
              <div class="absolute" :style="{'background-image':'url('+require('@/assets/images/4124936_1-thumb-450x450.png')+')'}">
              </div>
              <div class="w-450 absolute bottom-0 opacity-0 transition-all duration-500 right-0 group-hover:opacity-100 border">
                
                <button class="bg-red-500 rounded-md">page</button><br/>
                <button class="bg-pink-500 rounded-md">git</button>
              </div>
          </div>
      </div> -->