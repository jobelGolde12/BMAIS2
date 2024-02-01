<template>
    <div v-if="showSidenav">
      <!-- <BmaisMainContent /> -->
        <div class="sidenav-header pt-2 d-flex gap-2 align-items-center">
            <div class="a-logo d-flex flex-row justify-content-center align-items center text-light">A</div>
            <div class="administrator-text">Administrator</div>
        </div>
    

    <div class="home mb-2">
      <div class="ul">
        <span><i class="bi bi-caret-right me-2"></i> <i class="bi bi-caret-down me-2" v-if="isCliked"></i></span>
       <a href="#" @click="toggleClick"> <i class="bi bi-house"></i>  Home</a>
       </div>  
      <div class="li-home" v-if="isClicked">
      <div><a href="#"><i class="bi bi-house me-1"></i> Home</a></div>  
      <div><a href="#"><i class="bi bi-megaphone me-1"></i> Announcement or News</a></div>  
      <div ><a href="#"> <i class="bi bi-tools me-2"> </i>Services</a></div>  
      <div><a href="#"><i class="bi bi-phone me-2"></i>Directory or Contacts</a></div>  
      <div><a href="#"><i class="bi bi-people-fill"></i> Community Resources</a></div>
      </div>  

    </div>

     <div class="barangay-officials mb-2">
      <div class="ul">
        <span><i class="bi bi-caret-right me-2" v-if="!isClicked2"></i> <i class="bi bi-caret-down me-2" v-if="isClicked2"></i></span>
        <i class="bi bi-people"></i> <a href="#" @click="toggleBarangayOfficial">Barangay officials</a></div>  
      <div class="li-home" v-if="isClicked2">
      <div><a href="#"><i class="bi bi-person me-1"></i> Barangay captain</a></div>  
      <div ><a href="#"> <i class="bi bi-tools me-2"> </i>Council member</a></div>  
      <div><a href="#"><i class="bi bi-phone me-2"></i>Watch man</a></div>  
      </div>  
    </div>

     <div class="staff mb-2">
      <div class="ul">
        <span><i class="bi bi-caret-right me-2" v-if="!isClicked3"></i> <i class="bi bi-caret-down me-2" v-if="isClicked3"></i></span>
        <i class="bi bi-person"></i> <a href="#" @click="toggleStaff">Staff</a></div>  
      <div class="li-home" v-if="isClicked3">
      <div><a href="#"><i class="bi bi-person me-1"></i> Barangay captain</a></div>  
      <div ><a href="#"> <i class="bi bi-tools me-2"> </i>Council member</a></div>  
      <div><a href="#"><i class="bi bi-phone me-2"></i>Watch man</a></div>  
      </div>  
    </div>

     <div class="purok-leader mb-2">
      <div class="ul">
        <span><i class="bi bi-caret-right me-2" v-if="!isClicked4"></i> <i class="bi bi-caret-down me-2" v-if="isClicked4"></i></span>
        <i class="bi bi-people"></i> <a href="#" @click="togglePurokLeader">Purok leader</a></div>  
      <div class="li-home" v-if="isClicked4">
      <div><a href="#"><i class="bi bi-person me-1"></i> Barangay captain</a></div>  
      <div ><a href="#"> <i class="bi bi-tools me-2"> </i>Council member</a></div>  
      <div><a href="#"><i class="bi bi-phone me-2"></i>Watch man</a></div>  
      </div>  
    </div>

      <div class="project-management mb-2">
      <div class="ul">
        <span><i class="bi bi-caret-right me-2" v-if="!isClicked5"></i> <i class="bi bi-caret-down me-2" v-if="isClicked5"></i></span>
        <i class="bi bi-people"></i> <a href="#" @click="toggleProjectManagement">Project Management</a></div>  
      <div class="li-home" v-if="isClicked5">
      <div><a href="#"><i class="bi bi-plus me-1"></i> Create new</a></div>  
      <div ><a href="#"> <i class="bi bi-list me-2"> </i>Project list view</a></div>  
      <div><a href="#"><i class="bi bi-phone me-2"></i>Project board view</a></div>  
      <div><a href="#"><i class="bi bi-phone me-2"></i>Project Todo list</a></div>  
      <div><a href="#"><i class="bi bi-phone me-2"></i>Project details</a></div>  

      </div>  
    </div>


    <div class="activities mb-2">
      <a href="#"><i class="bi bi-activity me-2"></i>Activities</a>
    </div>

    <div class="household mb-2">
      <a href="#"><i class="bi bi-houses me-2"></i>Household</a>
    </div>

    <div class="contact mb-2">
      <a href="#"><i class="bi bi-telephone me-2"></i>Contact</a>
    </div>

   <i class="_sidenav-btn bi bi-list fs-3 text-primary" @click="toggleSidenav"></i>
    </div>
</template>

<script>
// import BmaisMainContent from './BmaisMainContent.vue'
export default{
 data(){
    return{
        isCliked: false,
        isClicked2: false,
        isClicked3: false,
        isClicked4: false,
        isClicked5: false,
        showSidenav: true
    }
 },

 methods:{
    toggleClick(){
        this.isCliked = !this.isCliked
    },

    toggleBarangayOfficial(){
        this.isClicked2 = !this.isClicked2
    },
    
    toggleStaff(){
        this.isClicked3 = !this.isClicked3
    },
    togglePurokLeader(){
        this.isClicked4 = !this.isClicked4
    },
    toggleProjectManagement(){
        this.isClicked5 = !this.isClicked5
    },
    toggleSidenav(){
      this.showSidenav = !this.showSidenav
    }

 }
}

</script>
