<template>
<div class="contact">
    <div class=" container-fluid mt-5 ms-2 ">
        <div>
            <h1 class="text-muted mb-0">Contact</h1>
        <p class="text-muted">Direct contact to a person</p>
        </div>
      
      <div class="container-fluid contact-header mt-4">
        <ul class="d-flex gap-3">
            <li class="text-center">
                <img src="../assets/my-profile.jpg" alt="">
                <p class="text-dark username">Jobel</p>
            </li>

            <li class="text-center">
                <img src="../assets/andre.jpg" alt="">
                <p class="text-dark username">Andre</p>
            </li>

            <li class="text-center">
                <img src="../assets/peter.jpg" alt="">
                <p class="text-dark username">Peter</p>
            </li>

            <li class="text-center">
                <img src="../assets/welbert.jpg" alt="">
                <p class="text-dark username">Welbert</p>
            </li>

            <li class="text-center">
                <img src="../assets/jose.jpg" alt="">
                <p class="text-dark username">Jose</p>
            </li>

            <li class="text-center">
                <img src="../assets/rema.jpg" alt="">
                <p class="text-dark username">Rema</p>
            </li>

            <li class="text-center">
                <img src="../assets/profile1.jpg" alt="">
                <p class="text-dark username">Joela</p>
            </li>

            <li class="text-center">
                <img src="../assets/tamon.jpg" alt="">
                <p class="text-dark username">Tamon</p>
            </li>

            <li class="text-center">
                <img src="../assets/profile2.jpg" alt="">
                <p class="text-dark username">Rexielyn</p>
            </li>

            <li class="text-center">
                <img src="../assets/profile3.jpg" alt="">
                <p class="text-dark username">Lily</p>
            </li>

        </ul>
      </div>

      <div class="container group-chat-container">
        <h5 class="text-dark mb-3">Group Chats</h5>

        <div class="card  mt-3">
           <div class="card-header d-flex flex-row gap-2 align-items-center">
            <div> <img src="../assets/profile4.jpg" alt="" class="profile-image"></div>
            <div><p class="text-dark fw-bold mt-2">Project waste management GC.</p></div>
           </div>
           <div class="card-body d-flex flex-row gap-2 align-items-center justify-content-between">
            <div class="current-chat mt-3 d-flex align-items-center gap-2">
              <div><p class="current-chat-person text-dark fw-bold">Kagawad:</p></div>
            <div class="mb-3">may meeting po k... </div>
            </div>
            <div class="d-flex button-handler">
                <button class="btn btn-primary me-3 ms-5"> <i class="bi bi-eye me-1"></i>View</button>
                <button class="btn btn-warning"><i class="bi bi-trash"></i> Delete</button>
            </div>
           </div>
        </div>

        <div class="card  mt-3">
           <div class="card-header d-flex flex-row gap-2 align-items-center">
            <div> <img src="../assets/logo.png" alt="" class="profile-image"></div>
            <div><p class="text-dark fw-bold mt-2">Christmass group</p></div>
           </div>
           <div class="card-body d-flex flex-row gap-2 align-items-center justify-content-between">
            <div class="current-chat mt-3 d-flex align-items-center gap-2">
              <div><p class="current-chat-person text-dark fw-bold">Alder:</p></div>
            <div class="mb-3">2k po lahat </div>
            </div>
            <div class="d-flex button-handler">
                <button class="btn btn-primary me-3 ms-5"> <i class="bi bi-eye me-1"></i>View</button>
                <button class="btn btn-warning"><i class="bi bi-trash"></i> Delete</button>
            </div>
           </div>
        </div>

        <div class="card  mt-3">
           <div class="card-header d-flex flex-row gap-2 align-items-center">
            <div> <img src="../assets/logo.png" alt="" class="profile-image"></div>
            <div><p class="text-dark fw-bold mt-2">Mga kagawad</p></div>
           </div>
           <div class="card-body d-flex flex-row gap-2 align-items-center justify-content-between">
            <div class="current-chat mt-3 d-flex align-items-center gap-2">
              <div><p class="current-chat-person text-dark fw-bold">Peter:</p></div>
            <div class="mb-3">Ahh. opo Kahapon... </div>
            </div>
            <div class="d-flex button-handler">
                <button class="btn btn-primary me-3 ms-5"> <i class="bi bi-eye me-1"></i>View</button>
                <button class="btn btn-warning"><i class="bi bi-trash"></i> Delete</button>
            </div>
           </div>
        </div>


        <div class="card  mt-3">
           <div class="card-header d-flex flex-row gap-2 align-items-center">
            <div> <img src="../assets/logo.png" alt="" class="profile-image"></div>
            <div><p class="text-dark fw-bold mt-2">Team YEY</p></div>
           </div>
           <div class="card-body d-flex flex-row gap-2 align-items-center justify-content-between">
            <div class="current-chat mt-3 d-flex align-items-center gap-2">
              <div><p class="current-chat-person text-dark fw-bold">Leader:</p></div>
            <div class="mb-3">Kaya natin to! </div>
            </div>
            <div class="d-flex button-handler">
                <button class="btn btn-primary me-3 ms-5"> <i class="bi bi-eye me-1"></i>View</button>
                <button class="btn btn-warning"><i class="bi bi-trash"></i> Delete</button>
            </div>
           </div>
        </div>


    </div>
      <div class="right p-2">
       <div class="container">
        <div class="d-flex flex-row ms-3">
        <input type="text" id="searchContact" class="form-control mt-2" placeholder="Search contact...">
        <i class="bi bi-search fs-5 fw-bold search-contact"></i>
        </div>
        <h5 class="text-dark mt-3 mb-3 ms-3">Contact history</h5>

        <div class="container contact-history d-flex gap-2 align-items-center mt-3">
            <div><img src="../assets/andre.jpg" alt="" class="profile-image"></div>
            <div>
                
              <div><p class="text-dark fw-bold mb-0">Andre D. Gerona</p></div>
              <div class="message mt-0">Hi, major told me that he will visit...</div>
            </div>
        </div>


        <div class="container contact-history d-flex gap-2 align-items-center mt-3">
            <div><img src="../assets/profile4.jpg" alt="" class="profile-image"></div>
            <div>
                
              <div><p class="text-dark fw-bold mb-0">Barangay captain</p></div>
              <div class="message mt-0">Don't forget to announce about ou...</div>
            </div>
        </div>


        <div class="container contact-history d-flex gap-2 align-items-center mt-3">
            <div><img src="../assets/profile5.jpg" alt="" class="profile-image"></div>
            <div>
                
              <div><p class="text-dark fw-bold mb-0">Secretary</p></div>
              <div class="message mt-0">Our project done?</div>
            </div>
        </div>


        <div class="container contact-history d-flex gap-2 align-items-center mt-3">
            <div><img src="../assets/profile6.jpg" alt="" class="profile-image"></div>
            <div>
                
              <div><p class="text-dark fw-bold mb-0">Alder</p></div>
              <div class="message mt-0">I have another idea</div>
            </div>
        </div>


        <div class="container contact-history d-flex gap-2 align-items-center mt-3">
            <div><img src="../assets/welbert.jpg" alt="" class="profile-image"></div>
            <div>
                
              <div><p class="text-dark fw-bold mb-0">Welbert Doque</p></div>
              <div class="message mt-0">We are targeting to finish the pro...</div>
            </div>
        </div>


        <div class="container contact-history d-flex gap-2 align-items-center mt-3">
            <div><img src="../assets/profile1.jpg" alt="" class="profile-image"></div>
            <div>
                
              <div><p class="text-dark fw-bold mb-0">Peter Estucado</p></div>
              <div class="message mt-0">Ok then!</div>
            </div>
        </div>
       </div>
      </div>
    </div>

   
</div>
</template>

<style lang="css" scoped>
@import "./styles/global.css";
.contact-header{
    transform:translateX(-25%);
    max-width: 70%;

}
.contact-header li img , .profile-image{
    width: 60px;
    height: 60px;
    border-radius: 50%;
    background: #000;
}
.contact-header li{
    list-style: none;
}
.contact-header ul::-webkit-scrollbar {
    display: none;
}
.right{
    position: absolute;
    max-width: 30%;
    background: var(--bg-primary);
    right: 2%;
    height: 90%;
    top: 10%;
    overflow-y: scroll;
}
.search-contact{
    transform: translate(-150%,25%);
}
.search-contact:hover{
    color: var(--clr-in-hover);
}
.current-chat-person{
    font-size: .9rem;
}
.contact-header ul{
    overflow-x: scroll;

}
.group-chat-container{
    position: absolute;
    overflow-y: scroll;
    height: 50%;
}
.group-chat-container .card{
    position: relative;
    width: 45%;
}

</style>
