<template>
<div>
    <div class="container-fluid mt-5 ms-2 ">
        <div>
            <h1 class="text-muted mb-0">Contact</h1>
        <p class="text-muted">Direct contact to a person</p>
        </div>
      
      <div class="container-fluid contact-header mt-4">
        <ul class="d-flex gap-3">
            <li class="text-center">
                <img src="../assets/logo.png" alt="">
                <p class="text-dark username">Jobel</p>
            </li>

            <li class="text-center">
                <img src="../assets/logo.png" alt="">
                <p class="text-dark username">Andre</p>
            </li>

            <li class="text-center">
                <img src="../assets/logo.png" alt="">
                <p class="text-dark username">Peter</p>
            </li>

            <li class="text-center">
                <img src="../assets/logo.png" alt="">
                <p class="text-dark username">Welbert</p>
            </li>

            <li class="text-center">
                <img src="../assets/logo.png" alt="">
                <p class="text-dark username">Alder</p>
            </li>

            <li class="text-center">
                <img src="../assets/logo.png" alt="">
                <p class="text-dark username">Ronel</p>
            </li>

            <li class="text-center">
                <img src="../assets/logo.png" alt="">
                <p class="text-dark username">Patrick</p>
            </li>
        </ul>
      </div>

      <div class="right p-2">
       <div class="container">
        <input type="text" id="searchContact" class="form-control mt-2" placeholder="Search contact...">
        <h5 class="text-dark mt-3 mb-3">Contact history</h5>

        <div class="container contact-history d-flex gap-2 align-items-center mt-3">
            <div><img src="../assets/logo.png" alt="" class="profile-image"></div>
            <div>
                
              <div><p class="text-dark fw-bold mb-0">Andre D. Gerona</p></div>
              <div class="message mt-0">Hi, major told me that he will visit...</div>
            </div>
        </div>


        <div class="container contact-history d-flex gap-2 align-items-center mt-3">
            <div><img src="../assets/logo.png" alt="" class="profile-image"></div>
            <div>
                
              <div><p class="text-dark fw-bold mb-0">Barangay captain</p></div>
              <div class="message mt-0">Don't forget to announce about ou...</div>
            </div>
        </div>


        <div class="container contact-history d-flex gap-2 align-items-center mt-3">
            <div><img src="../assets/logo.png" alt="" class="profile-image"></div>
            <div>
                
              <div><p class="text-dark fw-bold mb-0">Secretary</p></div>
              <div class="message mt-0">Our project done?</div>
            </div>
        </div>


        <div class="container contact-history d-flex gap-2 align-items-center mt-3">
            <div><img src="../assets/logo.png" alt="" class="profile-image"></div>
            <div>
                
              <div><p class="text-dark fw-bold mb-0">Alder</p></div>
              <div class="message mt-0">I have another idea</div>
            </div>
        </div>


        <div class="container contact-history d-flex gap-2 align-items-center mt-3">
            <div><img src="../assets/logo.png" alt="" class="profile-image"></div>
            <div>
                
              <div><p class="text-dark fw-bold mb-0">Welbert Doque</p></div>
              <div class="message mt-0">We are targeting to finish the pro...</div>
            </div>
        </div>


        <div class="container contact-history d-flex gap-2 align-items-center mt-3">
            <div><img src="../assets/logo.png" alt="" class="profile-image"></div>
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
.contact-header li img , .profile-image{
    width: 35px;
    height: 35px;
    border-radius: 50%;
    background: #000;
}
.contact-header li{
    list-style: none;
}
.right{
    position: absolute;
    max-width: 30%;
    background: var(--bg-primary);
    right: 2%;
    height: 80%;
    top: 10%;
    overflow-y: scroll;
}
    
</style>