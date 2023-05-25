<template>

  <div class="w-full px-[2%] sticky top-0 bg-white py-2.5 z-50">
    <div class="max-w-7xl mx-auto flex justify-between items-center">

        <button @click="$emit('MenuIndex','메인페이지')">
          <img src="http://via.placeholder.com/120x50" alt="img">
        </button>

        <div class="basis-3/4 md:block">
          <ul class="flex mx-auto">
            <li v-for="(e, index) in NavList[0]" :key="index">
              <!-- {{ langList.Nav[index] }} -->
              <button @click="$emit('MenuIndex',(index+1)+'페이지')" class="wando font-extrabold ml-5 text-2xl">
                {{ e }}
              </button>
            </li>
          </ul>
        </div>
    </div>
  </div>
  
</template>

<script>
import NavData from '../assets/Data.json'
  export default {
    name:"NavPage",
    data() {
      return {
        NavList:NavData.Nav,
        windowScroll : window.scrollY
      }
    },
    
    props : {
      langList:Object,
    },
    
  }
</script>

<style>

</style>