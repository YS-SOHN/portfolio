<template>
  <!-- <div class="bg-yellow-500 h-[970px]">portfolio
    </div> -->
  
  
  <div>
    <div class="w-full">
      <div class="w-7xl mx-auto">
          <div class="w-2xl mx-auto flex justify-center gap-x-[2%] gap-y-10 flex-wrap border relative">

              <div class="relative group overflow-hidden">
                 <img src="@/assets/images/4124936_1-thumb-450x450.png" alt="" class="rounded-md border hover:opacity-50">
                 <div class="absolute top-[30%] -right-10">
                   <button class="right-0 group-hover:opacity-100 group-hover:right-10 transition-all duration-500 opacity-0 absolute text-2xl">page</button><br>
                   <button class="right-0 group-hover:opacity-100 group-hover:right-10 transition-all duration-500 opacity-0 absolute text-2xl">git</button>
                 </div>
                 <div class="absolute w-[450px] bg-black opacity-50 h-[400px] -bottom-[450px] group-hover:bottom-0 transition-all duration-500">profile</div>
                 
              </div>

              
          </div>

      </div>

    </div>

  </div>

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




      <!-- <div :style="{ 'background-image': 'url(' + require('@/assets/images/4124936_1-thumb-450x450') + ')' }"></div> -->
  
</template>

<script>
  export default {
    name:'PortfolioPage',
    
  }
</script>

<style>

</style>