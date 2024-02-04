<template>
 <div>
    <div class="container-fluid _announcement-header d-flex flex-row justify-content-between align-items-center mt-5 ps-4 pe-2">
        <div class="header-content"><h5>Announcement</h5></div>
        <div class="header-search">
            <input type="text" placeholder="Search announcement..." class="ps-3 pe-5 pt-2 pb-2 rounded">
            <i class="bi bi-search fs-5 fw-bold"></i>
        </div>

        <div class="header-date">
            <input type="date" class="form-control">
        </div>
    </div>

    <div class="container-fluid d-flex justify-content-between mt-5 align-items-center">
        <div class="d-flex gap-2">
            <div class="text-dark">Current date: </div>
            <div><p class="text-primary">{{ date }}, {{ day }} {{ year }}</p></div>
        </div>
        <button class="btn btn-primary _add-announcement-btn float-right ms-2">
            <i class="bi bi-plus text-light"></i>
            Add announcement
        </button>
    </div>

    <div class="container-fluid">
        <table class="table table-striped mt-4">
            <thead>
                <tr>
                    <th>Announcement</th>
                    <th>Who announced</th>
                    <th>Date</th>
                    <th>Update</th>
                    <th>Delete</th>
                </tr>
            </thead>

            <tbody>
                <tr v-for="(data,index) in announcementData" :key="index">
                    <td class="text-dark">{{ announcementData[index].announcement}}</td>
                    <td  class="text-dark">{{ announcementData[index].whoAnnounce}}</td>
                    <td  class="text-dark">{{ announcementData[index].announcementDate}}</td>
                    <td><button class="btn btn-primary"> <i class="bi bi-pen"></i>Update</button></td>
                    <td><button class="btn btn-warning"> <i class="bi bi-trash"></i>Delete</button></td>
                </tr>
            </tbody>
        </table>
    </div>
 </div>
</template>

<script>
export default {
    data(){
        return{
            date: null,
            day: null,
            year: null,
            announcementData: []
        }
    },
    methods: {
        getDate(){
            let getDate = new Date()
            this.day = getDate.getDay()
            this.year= getDate.getFullYear()
            let getMonth = ''
          switch (getDate.getMonth()) {
              case 0:
               getMonth = 'January'
              break;
              case 1:
               getMonth = 'Febuary'
              break;
              case 0:
               getMonth = 'March'
              break;
              case 0:
               getMonth = 'April'
              break;
              case 0:
               getMonth = 'May'
              break;
              case 0:
               getMonth = 'June'
              break;
              case 0:
               getMonth = 'July'
              break;
              case 0:
               getMonth = 'August'
              break;
              case 0:
               getMonth = 'September'
              break;
              case 0:
               getMonth = 'Occtober'
              break;
              case 0:
               getMonth = 'November'
              break;
              case 0:
               getMonth = 'December'
              break;
          
          }

            this.date = getMonth
        },
        announcementTableData(){
         class AnnouncenetDataObj{
            constructor(announcement,whoAnnounce,announcementDate){
                this.announcement = announcement
                this.whoAnnounce = whoAnnounce
                this.announcementDate = announcementDate
            }
         }
         
         let a1 = new AnnouncenetDataObj("Street cleaning program","Jobel v. Golde", "1/23/2024")
         let a2 = new AnnouncenetDataObj("Feeding program","Boggart Valdez", "1/25/2024")
         let a3 = new AnnouncenetDataObj("Barangay ayuda","kap Toby", "2/1/2024")

        this.announcementData.push(a1,a2,a3)
        }
    },
    mounted(){
        this.getDate(),
        this.announcementTableData()
    }
}
</script>
<style lang="css" scoped>
@import "./styles/global.css";
._announcement-header{
    width: 70vw;
}
.header-search input{
    border: 1px solid var(--clr-secondary);
}
.header-search i{
    position: absolute;
    transform: translate(-150% , 28%);
}
    
</style>