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

              <!-- <div v-for="(e,index) in Contents" :key="e" class="relative group overflow-hidden  gap-y-5 mb-5 md:w-[48%] lg:w-[32%] w-[99%] sm:mx-auto">
                   <img :src="require(`@/assets/images/port_${index}.png`)" alt="" class="rounded-md hover:opacity-50 group-hover:scale-105 transition-all w-[400px] mx-auto">
                   <div class="ml-28">
                     <h2 class="font-extrabold mt-3 text-xl mb-2">{{ e.title }}</h2>
                     <p>{{ e.tool }}</p>
                     <p class="flex"><span class="w-[70px] block">{{ e.desc[0].title }}</span><span>:{{ e.desc[0].title2 }}</span></p>
                     <p class="flex"><span class="w-[70px] block ">{{ e.desc2[0].title }}</span><span>:{{ e.desc2[0].title2 }}</span></p>
                     <p class="flex"><span class="w-[70px] block ">{{ e.desc3[0].title }}</span><span>:{{ e.desc3[0].title2 }}</span></p>
                     <p class="flex"><span class="w-[70px] block ">{{ e.desc4[0].title }}</span><span>:{{ e.desc4[0].title2 }}</span></p>
                   </div>
                   
                   <div class="flex justify-center mt-2">
                     <div class="flex bottom-0 mx-auto gap-x-3">

                    <button type="button" class="text-white bg-gradient-to-r from-[#ff4440] via-[#ff4440] to-[#ff4440] hover:bg-gradient-to-br focus:ring-4 focus:outline-none focus:ring-[#ff4440] dark:focus:ring-[#ff4440] shadow-lg shadow-[#ff4440]/50 dark:shadow-lg dark:shadow-green-800/80 font-medium rounded-lg text-sm px-5 py-2.5 text-center mr-2 mb-2 hover:scale-105 transition-all"><a :href="e.link" target="_blank">Move Into</a></button>

                    <button type="button" class="text-white bg-gradient-to-r from-[#164562] via-[#164562] to-[#164562] hover:bg-gradient-to-br focus:ring-4 focus:outline-none focus:ring-[#164562] dark:focus:ring-[#164562] shadow-lg shadow-[#164562]/50 dark:shadow-lg dark:shadow-[#164562]/80 font-medium rounded-lg text-sm px-5 py-2.5 text-center mr-2 mb-2 hover:scale-105 transition-all">git Hub</button>


                     </div>
                   </div>
                </div> -->



              <!-- <div class="pb-24 basis-full flex flex-wrap gap-x-3.5 justify-between">
                <div class="basis-full border rounded-md mb-20 relative flex flex-wrap items-center group" v-for="(e,index) in Contents" :key="e">
                  <div class="basis-full md:basis-2/4 group-odd:order-1 md:group-odd:order-1 md:group-even:order-2">
                    <img :src="require(`@/assets/images/port_${index}.png`)" alt="e.title" class="w-full p-2.5 h-[350px]" />
                  </div>
                  <div class="basis-full md:basis-2/4 md:group-even:left-14 md:group-odd:-left-14 group-odd:order-2 group-even:order-1 relative z-10 bg-gray-50 pl-20 pr-5 sm:pr-0 sm:pl-12 py-5 box-border ">
                    
                    <h3 class="py-5 font-bold">{{ e.title }}</h3>
                    <p>{{ e.tool }}</p>
                     <p class="flex"><span class="w-[70px] block">{{ e.desc[0].title }}</span><span>:{{ e.desc[0].title2 }}</span></p>
                     <p class="flex"><span class="w-[70px] block ">{{ e.desc2[0].title }}</span><span>:{{ e.desc2[0].title2 }}</span></p>
                     <p class="flex"><span class="w-[70px] block ">{{ e.desc3[0].title }}</span><span>:{{ e.desc3[0].title2 }}</span></p>
                     <p class="flex"><span class="w-[70px] block ">{{ e.desc4[0].title }}</span><span>:{{ e.desc4[0].title2 }}</span></p>
                  </div>
                </div>
              </div> -->

              <div class="pb-24 basis-full flex flex-wrap gap-x-3.5">
                <div class="basis-full border rounded-md mb-5 flex flex-wrap group" v-for="(e,index) in Contents" :key="e">
                  <div class="basis-full sm:basis-2/4 group-odd:order-1 md:group-odd:order-1 md:group-even:order-2"><a :href="e.link">
                    <img :src="require(`@/assets/images/port_${index}.png`)" alt="e.title" class="w-full p-2.5 hover:scale-105 transition-all duration-700 border-2 border-red-500 rounded-md" />
                  </a>
                  </div>
                  <div class="basis-full sm:basis-2/4 pl-5 box-border group-odd:order-2 group-even:order-1 mt-10">
                    <h3 class="py-5 font-bold">{{ e.title }}</h3>
                    <p>{{ e.tool }}</p>
                     <p class="flex"><span class="w-[70px] block">{{ e.desc[0].title }}</span><span>:{{ e.desc[0].title2 }}</span></p>
                     <p class="flex"><span class="w-[70px] block ">{{ e.desc2[0].title }}</span><span>:{{ e.desc2[0].title2 }}</span></p>
                     <p class="flex"><span class="w-[70px] block ">{{ e.desc3[0].title }}</span><span>:{{ e.desc3[0].title2 }}</span></p>
                     <p class="flex"><span class="w-[70px] block ">{{ e.desc4[0].title }}</span><span>:{{ e.desc4[0].title2 }}</span></p>
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