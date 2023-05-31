<template>
    <div class="max-w-7xl p-5 mx-auto bg-white rounded-md darkMode">
      <p class="relative mx-auto text-center mb-14 oa text-3xl after:absolute after:w-10 after:h-0.5  after:bg-red-500 after:left-2/4 after:-translate-x-2/4 after:bottom-0 w-[220px] h-[50px] mt-14">{{ title }}</p>
      <!-- <h3 class="relative after:absolute after:w-2 after:h-[2px] after:bg-black after:dark:bg-[#d9d9d9] after:-bottom-1 after:left-2/4 after:-translate-x-2/4 tracking-widest text-center text-xl sm:text-2xl lg:text-3xl font-bold"></h3> -->
    </div>
  </template>
  
  <script>
  export default {
    name: "TitlePage",
    props:{
      title: String
    },
    data() {
      return {
        
      }
    },
  }
  </script>
  <style>
    
  </style>