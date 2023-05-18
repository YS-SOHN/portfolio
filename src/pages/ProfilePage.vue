<template>
  <div class="w-full text-white bg-[#164562] h-[970px] relative">profile
    <p class="relative mx-auto text-center mb-14 oa text-3xl after:absolute after:w-full after:h-2 after:bg-red-500 after:left-0 after:bottom-0 w-[220px] h-[50px]">ABOUT ME</p>
    <div class="max-w-7xl h-96 flex justify-center gap-x-[2%] mx-auto relative">
          <div class="w-[40%] h-48 border-red-500">
              <ul class="flex justify-between">
                <li><img src="http://via.placeholder.com/200" alt="img" /></li>
                <li class="border w-[60%] pl-2 ml-2 pt-1">
                    <h2 class="pt36 text-2xl">손 유상</h2>
                    <p>Yu-sang SOHN</p>
                    <p class="pt-3 text-lg">1987.06.27</p>
                    <p class="pt-3 text-lg">E-mail : sdg0627@gmail.com</p>
                </li>
              </ul>
            
          <div class="w-full">
            <div class="mt-5 border">
                <h3 class="text-2xl mt-3 mb-1">학력</h3>
                <p class="mb-1">계명대학교 입학 (화학공학과) 2006</p>
                <p class="flex flex-wrap overflow-hidden">Working Holiday </p>
                <p class="mb-1">Brisbane Aus. 12.07.22 ~ 13.07.22</p>
                <p class="mb-1">계명대학교 졸업 (화학공학과) 0000</p>
                <p class="flex flex-wrap overflow-hidden mb-1">(디지털컨버전스) 스마트 혼합-뷰(Vue) 활용 프론트엔드 개발자 양성과정 B 2022.12.29 ~ 2023.06.12</p>

            </div>
          </div>          
        </div>

        <div class="w-[40%] border h-full pl-2 pt-2">
            <h3 class="text-2xl">해외경험</h3>
            <p>(Australia) : Sydney, Melbourn, Tasmania, Brisbane</p>
            <p>(Japan) : Osaka, Kyoto</p>
            <p>(Taiwan) : Taipei</p>
        </div>
      </div>
  </div>
</template>

<script>
  export default {
    name:'ProfilePage'
    
  }
</script>

<style>

/* .background{
  width:100%;
  padding-bottom:100%;
  background-color:blue;
  top:0; left:0;
} */


</style>