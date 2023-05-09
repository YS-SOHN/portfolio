<template>
  

<NavMenu @MenuIndex="MenuIndex = $event;" @click="SectionMove()" @dark="event => toggleDark()" @lang="lang=$event" :langList="langList[lang]" />
  

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

<div class="fixed">
 {{ MenuIndex }}
  </div>
  

  
</template>

<script>
import Language from './assets/Language.json'
import Home from './pages/HomePage.vue'
import Profile from './pages/ProfilePage.vue'
import Skill from './pages/SkillPage.vue'
import NavMenu from './components/Nav.vue'
import Portfolio from './pages/PortfolioPage.vue'

export default {
  name: 'App',
  components: {
    Home,
    Profile,
    Skill,
    NavMenu,
    Portfolio
  },
  data() {
    return {
      MenuIndex:'메인페이지',
      langList:Language,
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
