<template>
 <HomeSection/>
 <BmaisNavbar />
 <div class="main d-flex flex-row">
   <BmaisSidenav class="sidenav ps-2" :toggleMainContent="getToggleMainContent" @toggleMainContentFunc="toggleMainContentFunc" :toggleAnnouncement="getToggleAnnouncement" @toggleAnnouncementFunc="toggleAnnouncementFunc" :toggleContact="toggleContact" @toggleContactFunc="toggleContactFunc"/>
 <BmaisMainContent class="main-content" v-if="getToggleMainContent"/>
 <BmaisAnnouncement v-if="getToggleAnnouncement"/>
 <BmaisContact v-if="toggleContact"/>
 </div>
</template>

<script>

import HomeSection from './components/HomeSection.vue'
import BmaisNavbar from './components/BmaisNavbar.vue'
import BmaisSidenav from './components/BmaisSidenav.vue'
import BmaisMainContent from './components/BmaisMainContent.vue'
import BmaisAnnouncement from './components/BmaisAnnouncement.vue'
import BmaisContact from './components/BmaisContact.vue';

export default {
  name: 'App',
  data(){
    return{
     getToggleMainContent: true,
     getToggleAnnouncement: false,
     toggleContact: false
    }
  },
 components: {
  HomeSection, BmaisNavbar,BmaisSidenav,BmaisMainContent,BmaisAnnouncement,BmaisContact
 },
 methods:{
  toggleMainContentFunc(newBoolean){
    this.getToggleMainContent = newBoolean
    this.getToggleAnnouncement = false
    this.toggleContact = false
  },
  toggleAnnouncementFunc(newBoolean){
    this.getToggleAnnouncement = newBoolean
    this.getToggleMainContent = false
    this.toggleContact = false
  },
  toggleContactFunc(){
    this.toggleContact = !this.toggleContact
    this.getToggleMainContent = false
    this.getToggleAnnouncement = false
  }
 }
}
</script>

<style>
@import "~bootstrap/dist/css/bootstrap.css";
@import "https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css";
@import "components/styles/global.css";
</style>
