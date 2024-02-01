<template>
    <div>
        <header class="header d-flex flex-row justify-content-between pt-2 ps-2 pe-2  align-items-center">
            <div class="logo"><h5>BMAIS</h5></div>
            <div class="search d-flex flex-row align-items-center">
                <input type="text" placeholder="Seach...">
                <i class="bi bi-search"></i>
            </div>

            <div class="navbar-right">
                <i class="bi bi-person me-4"></i>
                <i class="bi bi-list-task  me-4"></i>
                <span>
                    <i class="bi bi-sun  me-4" v-if="theme" @click="toggleTheme"></i>
                    <i class="bi bi-moon  me-4" v-if="!theme" @click="toggleTheme"></i>
                </span>

            </div>
        </header>
    </div>
</template>

<script>
export default {
  
    data(){
        return{
            theme: true
        }
    },
    methods: {
        toggleTheme(){
            this.theme = !this.theme
        }
    }
}
</script>

<style lang="css">
   @import "styles/global.css";
   .header .search input{
    padding: .2rem 1rem;
    border-radius: 20px;
    border: 1.5px solid var(--clr-secondary);
    width:100%;
   }
   .search{
    width: 30%;
   }
   .logo{
    color: var(--clr-secondary);
   }
   .navbar-right i:hover{
    color: var(--clr-in-hover);

   }
   .search i{
    transform: translateX(-170%);
   }
   .search{
    margin-left: 9rem;
   }
</style>