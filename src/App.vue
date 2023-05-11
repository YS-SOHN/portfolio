<template>
  {{ Language }}
  
{{ lang }}
<NavMenu @MenuIndex="MenuIndex = $event;" @click="SectionMove()" :langList="langList[0]" />
  

  <div ref="메인페이지">
    <Home />
  </div>

<div ref="1페이지">
  <Profile  />
</div>

<div ref="2페이지"> 
  <Skill  />
</div>

<div ref="3페이지"> 
  <Portfolio  />
</div>

<div ref="4페이지"> 
  <Life  />
</div>

<div class="fixed">
 {{ MenuIndex }}
  </div>
  

  
</template>

<script>
import NavData from '@/assets/Data.json'
import Home from './pages/HomePage.vue'
import Profile from './pages/ProfilePage.vue'
import Skill from './pages/SkillPage.vue'
import NavMenu from './components/Nav.vue'
import Portfolio from './pages/PortfolioPage.vue'
import Life from './pages/LifePage.vue'

export default {
  name: 'App',
  components: {
    Home,
    Profile,
    Skill,
    NavMenu,
    Portfolio,
    Life
  },
  data() {
    return {
      MenuIndex:'메인페이지',
      langList:NavData,
      ArrayList:'',
      lang:0
    }
  },
  methods :{
    SectionMove(){
      const rect = this.ArrayList[this.MenuIndex].getBoundingClientRect();
      const offset = rect.top + window.scrollY;
      window.scrollTo({
        top:offset,
        behavior:'smooth'
      })
      // console.log(this.MenuIndex)

    }
  },
  mounted(){
    this.ArrayList = this.$refs;
    console.log(this.ArrayList)
    
    
    
  }
}
</script>

<style>
  .duration {animation-duration: .5s;}
</style>
