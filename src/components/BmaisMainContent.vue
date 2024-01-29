<template>
    <div>
        <div class="main-content-header container d-flex flex-row justify-content-around mt-5">
         <div class="card bg-primary">
            <div class="card-body text-light"><i class="bi bi-megaphone me-2"></i>Announcement</div>
         </div>

         <div class="card bg-secondary">
            <div class="card-body text-light"><i class="bi bi-file-text me-2"></i> Report</div>
         </div>

         <div class="card bg-info cursor-pointer">
            <div class="card-body text-light"><i class="bi bi-people-fill me-2"></i>Resident's</div>
         </div>
        </div>

        <div>
    <div class="chart-container container-fluid">
        <canvas id="myChart" class="mt-4 container-fluid"></canvas>
    </div>
</div>

    </div>
</template>



<script>
export default {
    data(){
        return{
            name: ''
        }
    },
    methods: {
        getChart(){
            const ctx = document.getElementById('myChart');

  new Chart(ctx, {
    type: 'bar',
    data: {
      labels: ['Red', 'Blue', 'Yellow', 'Green', 'Purple', 'Orange'],
      datasets: [{
        label: '# of Votes',
        data: [12, 19, 3, 5, 2, 3],
        borderWidth: 1
      }]
    },
    options: {
      scales: {
        y: {
          beginAtZero: true
        }
      }
    }
  });
        }
    },
    mounted(){
        this.getChart()
    }
}
</script>

<style lang="css">
    .chart-container{
    height: 60vh;
    width: 100%;
    }
    .chart-container #myChart{
        position: relative;
        width: 100%;
    }
</style>