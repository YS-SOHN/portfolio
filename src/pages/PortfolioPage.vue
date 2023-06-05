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
      <Title title="PortPolio" />
      <div class="w-7xl mx-auto">
          <div class="max-w-7xl mx-auto flex justify-center flex-wrap relative">
            <div class="flex flex-wrap gap-x-[2%]">
              <div v-for="(e,index) in Contents" :key="e" class="relative group overflow-hidden  gap-y-5 mb-5 md:w-[48%] lg:w-[32%] w-[99%] sm:mx-auto">
                   <img :src="require(`@/assets/images/port_${index}.png`)" alt="" class="rounded-md hover:opacity-50 group-hover:scale-105 transition-all w-[400px] mx-auto">
                   <div>
                     <h2 class="font-extrabold mt-3">{{ e.title }}</h2>
                     <p><span>{{ e.desc[0].title }}</span><span>{{ e.desc[0].title2 }}</span></p>
                     <p><span>{{ e.desc2[0].title }}</span><span>{{ e.desc2[0].title2 }}</span></p>
                     <p><span>{{ e.desc3[0].title }}</span><span>{{ e.desc3[0].title2 }}</span></p>
                     <p><span>{{ e.desc4[0].title }}</span><span>{{ e.desc4[0].title2 }}</span></p>
                     <p>{{ e.tool }}</p>
                   </div>
                   
                   <div class="flex justify-center mt-2">
                     <div class="flex bottom-0 mx-auto gap-x-3">

                    <button type="button" class="text-white bg-gradient-to-r from-green-400 via-green-500 to-green-600 hover:bg-gradient-to-br focus:ring-4 focus:outline-none focus:ring-green-300 dark:focus:ring-green-800 shadow-lg shadow-green-500/50 dark:shadow-lg dark:shadow-green-800/80 font-medium rounded-lg text-sm px-5 py-2.5 text-center mr-2 mb-2"><a :href="e.link" target="_blank">Move Into</a></button>

                    <button type="button" class="text-white bg-gradient-to-r from-pink-400 via-pink-500 to-pink-600 hover:bg-gradient-to-br focus:ring-4 focus:outline-none focus:ring-pink-300 dark:focus:ring-pink-800 shadow-lg shadow-pink-500/50 dark:shadow-lg dark:shadow-pink-800/80 font-medium rounded-lg text-sm px-5 py-2.5 text-center mr-2 mb-2">git Hub</button>


                     </div>
                   </div>
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
  import Title from '@/components/Title.vue'

  export default {
    components: {
      // Swiper,
      // SwiperSlide,
      Title
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