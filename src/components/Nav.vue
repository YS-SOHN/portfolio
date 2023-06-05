<template>
  <div>
  <div class="w-full px-[2%] fixed top-0 bg-white/50 py-2.5 z-50 ">
    <div class="max-w-7xl mx-auto flex justify-between items-center ">
        <div>
          <button @click="$emit('MenuIndex','메인페이지')">
          <img src="http://via.placeholder.com/120" class="rounded-full" alt="img">
          </button>
        </div>
        

        <div class="basis-3/4 md:block">
          <ul class="flex mx-auto flex-basis justify-center gap-x-10 ">
            <li v-for="(e, index) in NavList" :key="index" class="nanum text-base">
              <!-- {{ langList.Nav[index] }} -->
              <button @click="$emit('MenuIndex',(index+1)+'페이지')" class="wando ml-5 font-semibold">
                {{ e }}
              </button>
            </li>
          </ul>
        </div>

        <div class="Vertical Align">
          <div class="flex gap-x-3 mb-2">
              <img src="git.png" alt="" class="w-10 h-10">
              <img src="html.png" alt="" class="w-10 h-10">
            </div>
            <div class="flex gap-x-3">
              <img src="css.png" alt="" class="w-10 h-10">
              <img src="js.png" alt="" class="w-10 h-10 rounded-lg">
          </div>
        </div>
        
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
@font-face {
    font-family: 'NanumSquareNeo-Variable';
    src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_11-01@1.0/NanumSquareNeo-Variable.woff2') format('woff2');
    font-weight: normal;
    font-style: normal;
}


.nanum {font-family: 'NanumSquareNeo-Variable';}

</style>