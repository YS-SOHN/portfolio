<template>
  <div class="w-full px-[2%] sticky top-0 bg-white py-2.5 z-50">
    <div class="max-w-7xl mx-auto flex justify-between items-center">

        <button @click="$emit('MenuIndex','메인페이지')">
          <img src="http://via.placeholder.com/120x50" alt="img">
        </button>

        <div class="basis-3/4 hidden md:block">
          <ul class="flex justify-around">
            <li v-for="(e, index) in NavList[0]" :key="index">
              <!-- {{ langList.Nav[index] }} -->
              <button @click="$emit('MenuIndex',(index+1)+'페이지') ">
                {{ langList.Nav[index] }}
              </button>
            </li>
          </ul>
        </div>
    </div>
  </div>
</template>

<script>
  export default {
    name:"NavPage",
    data() {
      return {
        NavList : [["프로필","스킬","포트폴리오"]]        
      }
    },
    props : {
      langList:Object
    }
  }
</script>

<style>

</style>