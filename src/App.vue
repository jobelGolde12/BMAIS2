<template>
 <HomeSection/>
 <BmaisNavbar />
 <div class="main d-flex flex-row">
   <BmaisSidenav class="sidenav ps-2" :toggleMainContent="getToggleMainContent" @toggleMainContentFunc="toggleMainContentFunc"/>
 <BmaisMainContent class="main-content" v-if="getToggleMainContent"/>
 </div>
</template>

<script>

import HomeSection from './components/HomeSection.vue'
import BmaisNavbar from './components/BmaisNavbar.vue'
import BmaisSidenav from './components/BmaisSidenav.vue'
import BmaisMainContent from './components/BmaisMainContent.vue'


export default {
  name: 'App',
  data(){
    return{
     getToggleMainContent: null
    }
  },
 components: {
  HomeSection, BmaisNavbar,BmaisSidenav,BmaisMainContent
 },
 methods:{
  toggleMainContentFunc(newBoolean){
    this.getToggleMainContent = newBoolean
  }
 }
}
</script>

<style>
@import "~bootstrap/dist/css/bootstrap.css";
@import "https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css";
@import "components/styles/global.css";
</style>
