<template>
 <HomeSection />
 <BmaisNavbar />
 <BmaisSidenav class="sidenav"/>
 <BmaisMainContent class="main-content"/>
</template>

<script>

import HomeSection from './components/HomeSection.vue'
import BmaisNavbar from './components/BmaisNavbar.vue'
import BmaisSidenav from './components/BmaisSidenav.vue'
import BmaisMainContent from './components/BmaisMainContent.vue'



export default {
  name: 'App',
 components: {
  HomeSection, BmaisNavbar,BmaisSidenav,BmaisMainContent
 }
}
</script>

<style>
@import "~bootstrap/dist/css/bootstrap.css";
@import url("https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css");
@import "../componets/styles/homesectionstyle.css";
</style>
