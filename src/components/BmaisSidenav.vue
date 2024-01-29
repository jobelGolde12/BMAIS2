<template>
    <div>
        <div class="sidenav-header pt-2 d-flex gap-2 align-items-center">
            <div class="a-logo d-flex flex-row justify-content-center align-items center text-light">A</div>
            <div class="administrator-text">Administrator</div>
        </div>
    

    <div class="home">
      <div class="ul"><i class="bi bi-house"></i> <a href="#" @click="toggleClick">Home</a></div>  
      <div class="li-home" v-if="isCliked">
      <div><a href="#"><i class="bi bi-megaphone me-1"></i> Announcement or News</a></div>  
      <div ><a href="#"> <i class="bi bi-tools me-2"> </i>Services</a></div>  
      <div><a href="#"><i class="bi bi-phone me-2"></i>Directory or Contacts</a></div>  
      <div><a href="#"><i class="bi bi-people-fill"></i> Community Resources</a></div>
      </div>  

    </div>

     <div class="home">
      <div class="ul"><i class="bi bi-house"></i> <a href="#" @click="toggleClick">Home</a></div>  
      <div class="li-home" v-if="isCliked">
      <div><a href="#"><i class="bi bi-megaphone me-1"></i> Announcement or News</a></div>  
      <div ><a href="#"> <i class="bi bi-tools me-2"> </i>Services</a></div>  
      <div><a href="#"><i class="bi bi-phone me-2"></i>Directory or Contacts</a></div>  
      <div><a href="#"><i class="bi bi-people-fill"></i> Community Resources</a></div>
      </div>  

    </div>

     <div class="home">
      <div class="ul"><i class="bi bi-house"></i> <a href="#" @click="toggleClick">Home</a></div>  
      <div class="li-home" v-if="isCliked">
      <div><a href="#"><i class="bi bi-megaphone me-1"></i> Announcement or News</a></div>  
      <div ><a href="#"> <i class="bi bi-tools me-2"> </i>Services</a></div>  
      <div><a href="#"><i class="bi bi-phone me-2"></i>Directory or Contacts</a></div>  
      <div><a href="#"><i class="bi bi-people-fill"></i> Community Resources</a></div>
      </div>  

    </div>

     <div class="home">
      <div class="ul"><i class="bi bi-house"></i> <a href="#" @click="toggleClick">Home</a></div>  
      <div class="li-home" v-if="isCliked">
      <div><a href="#"><i class="bi bi-megaphone me-1"></i> Announcement or News</a></div>  
      <div ><a href="#"> <i class="bi bi-tools me-2"> </i>Services</a></div>  
      <div><a href="#"><i class="bi bi-phone me-2"></i>Directory or Contacts</a></div>  
      <div><a href="#"><i class="bi bi-people-fill"></i> Community Resources</a></div>
      </div>  

    </div>

     <div class="home">
      <div class="ul"><i class="bi bi-house"></i> <a href="#" @click="toggleClick">Home</a></div>  
      <div class="li-home" v-if="isCliked">
      <div><a href="#"><i class="bi bi-megaphone me-1"></i> Announcement or News</a></div>  
      <div ><a href="#"> <i class="bi bi-tools me-2"> </i>Services</a></div>  
      <div><a href="#"><i class="bi bi-phone me-2"></i>Directory or Contacts</a></div>  
      <div><a href="#"><i class="bi bi-people-fill"></i> Community Resources</a></div>
      </div>  

    </div>

    </div>
</template>

<script>
export default{
 data(){
    return{
        isCliked:false
    }
 },

 methods:{
    toggleClick(){
        this.isCliked = !this.isCliked
    }
 }
}

</script>
