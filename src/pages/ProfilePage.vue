<template>
  <div class="w-full text-white bg-[#164562] h-[970px] relative pt-[170px]">

      <div class="flex justify-center gap-x-28 pt-24 items-center">
          <div>
            <!-- 사진 -->
            <img src="http://via.placeholder.com/120" alt="" class="rounded-full">
          </div>
          <div class="w-1 h-36 bg-red-500">

          </div>
          <div>
              <h1>손유상</h1>
              <h3>Yu-sang SOHN</h3>
              <h4>sdg0627@naver.com</h4>
          </div>
      </div>

      <div class="items-center max-w-7xl mx-auto mt-20 flex gap-x-7">
        <!-- education -->
        <div class="relative before:absolute before:-top-4 before:-left-4 before:w-4 before:h-4 before:bg-red-500 font-semibold text-lg">Education
            <div class="items-center flex">
              <!-- Education -->
              <span class="text-3xl font-extrabold mr-7">2022</span>
              <div class="items-center">
                <p>(디지털컨버전스)스마트 혼합-뷰(vue)활용</p>
                <p>프론트엔드 개발자 양성과정B 22.12.29~23.06.12</p>
              </div>
            </div>
            <div class="items-center flex">
              <!-- Education -->
              <span class="text-3xl font-extrabold mr-7">2009</span>
              <div class="items-center">
                <p>Working Holiday | Brisbane Aus.</p>
              </div>
            </div>
            <div class="items-center flex">
              <!-- Education -->
              <span class="text-3xl font-extrabold mr-7">2006</span>
              <div class="items-center">
                <p>계명대학교 (화학공학) 2006~2012</p>
              </div>
            </div>
        </div>

        <div class="mt-4 text-[#164562] font-extrabold text-2xl">
          <!-- chana -->
          <div class="flex gap-x-4 mb-4">
              <div class="bg-[#236892] w-44 h-[90px] rounded-lg pl-2">AUSTRALIA  
                 <ul class="flex flex-wrap">
                    <li class="text-xs">Sydney |&nbsp;</li>
                    <li class="text-xs">Melbourne |&nbsp;</li>
                    <li class="text-xs">Tasmania |&nbsp;</li>
                    <li class="text-xs">Brisbane |&nbsp;</li>
                    <li class="text-xs">GoldCoast</li>
                 </ul>
                </div>
              <div class="bg-[#236892] w-44 h-[90px] rounded-lg pl-2">JAPAN
                  <ul class="flex flex-wrap">
                      <li class="text-xs">Osaka |&nbsp;</li>
                      <li class="text-xs">Kyoto</li>
                  </ul>
              </div>
          </div>
          <div class="flex gap-4">
              <div class="bg-[#236892] w-44 h-[90px] rounded-lg pl-2 flex flex-wrap">CHINA
                <ul class="flex flex-wrap">
                  <li class="text-xs">Beijing |&nbsp;</li>
                    <li class="text-xs">Yanbian |&nbsp;</li>
                    <li class="text-xs">Yanji</li>
                </ul>
              </div>
              <div class="bg-[#236892] w-44 h-[90px] rounded-lg pl-2 flex flex-wrap">TAIWAN
                  <div class="text-xs basis-full">Taipei</div>
              </div>
          </div>
        </div>
        
        <div>
          <!-- licence -->
            <h2 class="font-extrabold text-xl mb-2">Licence</h2>
            <div class="mb-1">
                <p class="font-bold">2023.00</p>
                <p class="font-light">워드프로세서 1급</p>
            </div>
            <div class="mb-1">
                <p class="font-extrabold">2023.00</p>
                <p class="font-light">정보처리기능사</p>
            </div>
            <div>
                <p class="font-extrabold">2023.00</p>
                <p class="font-light">컴퓨터활용능력 2급</p>
            </div>
        </div>
      </div>
    
  </div>
</template>

<script>

  export default {
    name:'ProfilePage',

    data() {
      return {
        contents : [
          {
            title : "Education",
            desc: "계명대학교 (화학공학과) 2006 ~ 2012",
            desc2:"Working Holiday :Brisbane Aus.",
            desc3:"(디지털컨버전스) 스마트 혼합-뷰(vue) 활용 ",
            desc4:"프론트엔드 개발자 양성과정B 2022.12.29~23.06.12"
          },
          {
            title:"Overseas Experience",
            desc:"Australia : Sydney, Melbourne, Tasmania, Brisbane, GoldCoase",
            desc2:"Japan : Osaka, Kyoto",
            desc3 : "Taiwan : Taipei",
            desc4 : "China : Beijing, Yanbian, Yanji "
          },
          {
            title:"LICENCE",
            desc:"워드프로세서 1급",
            desc2:"정보처리기능사",
            desc3:"컴퓨터활용능력 2급"
          },
          {
            title:"Hobby",
            desc:"MTB, RoadBike",
            desc2:"국내외 여행",
            desc3:"",
          }
        ]
      }
    },
    
    
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