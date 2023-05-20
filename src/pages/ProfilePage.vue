<template>
  <div class="w-full text-white bg-[#164562] h-[970px] relative ">profile
    <p class="relative mx-auto text-center mb-14 oa text-3xl after:absolute after:w-full after:h-2 after:bg-red-500 after:left-0 after:bottom-0 w-[220px] h-[50px] mt-14">ABOUT ME</p>

    <div class="max-w-4xl h-96 flex justify-around gap-x-[2%] mx-auto relative flex-wrap">
      <div>
          <img src="http://via.placeholder.com/150x150" alt="">
          <ul class="">
              <li>손유상</li>
              <li>1987 . 06 . 27</li>
              <li>E-mail : sdg0627@naver.com</li>
          </ul>
      </div>
      <div>
        <div v-for="e in contents" :key="e" class="mb-5">
              <h3 class="text-xl font-extrabold mb-2">{{ e.title }}</h3>
              <p>{{ e.desc }}</p>
              <p>{{ e.desc1 }}</p>
              <p>{{ e.desc2 }}</p>
              <p>{{ e.desc3 }}</p>
              <p>{{ e.desc4 }}</p>
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
            desc: " - 계명대학교 (화학공학과) 2006 ~ 2012",
            desc2:" - Working Holiday :Brisbane Aus.",
            desc3:" - (디지털컨버전스) 스마트 혼합-뷰(vue) 활용 ",
            desc4:"프론트엔드 개발자 양성과정B 2022.12.29~23.06.12"
          },
          {
            title:"Overseas Experience",
            desc:" - Australia : Sydney, Melbourne, Tasmania, Brisbane, GoldCoase",
            desc2:" - Japan : Osaka, Kyoto",
            desc3 : " - Taiwan : Taipei"
          },
          {
            title:"LICENCE",
            desc:" - 워드프로세서 1급",
            desc2:" - 정보처리기능사",
            desc3:" - 컴퓨터활용능력 2급"
          },
          {
            title:"Hobby",
            desc:" - MTB, RoadBike",
            desc2:" - 국내외 여행",
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