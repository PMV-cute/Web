<template>
  <div class="main_cont1">
      <div class="middle_">
          <div class="circles_">
              <div class="circle_1">
                  <div class="circle_1_bar_1">
                      <img src="../assets/middle_circle1/Conversion.png" alt="1" class="img__">
                      <img src="../assets/middle_circle1/Small.png" alt="2" class="img__" style="cursor: pointer;">
                  </div>
                  <div class="items_">
                      <img src="../assets/middle_circle1/circleChart.png" alt="">
                  </div>
                  <div class="items_">
                      <img src="../assets/middle_circle1/item.png" alt="">
                      <img src="../assets/middle_circle1/item2.png" alt="">
                      <img src="../assets/middle_circle1/item3.png" alt="">
                  </div>
              </div>
              <div class="circle_1">
                  <div class="circle_1_bar_1">
                      <img src="../assets/middle_circle2/Users.png" alt="1" class="img__">
                      <img src="../assets/middle_circle1/Small.png" alt="2" class="img__" style="cursor: pointer;">
                  </div>
                  <div class="items_">
                      <img src="../assets/middle_circle2/circleChart.png" alt="">
                  </div>
                  <div class="items_">
                      <img src="../assets/middle_circle2/item.png" alt="">
                      <img src="../assets/middle_circle2/item2.png" alt="">
                      <img src="../assets/middle_circle2/item3.png" alt="">
                  </div>
              </div>
          </div>
          <div class="circles_">
              <div class="diagram_1">
                  <div class="circle_1_bar_1">
                      <img src="../assets/middle_diagram/Revenue.png" alt="1" class="img__">
                      <img src="../assets/middle_diagram/Small.png" alt="2" class="img__">
                  </div>
                  <div class="diagram_">
                      <img src="../assets/middle_diagram/chart.png" alt="" class="diagram_img">
                  </div>
                  <div class="middle_value">
                      <img src="../assets/middle_diagram/bottomvalue.png" alt="">
                  </div>
              </div>
          </div>
      </div>
  </div>

</template>

<script lang="ts">

</script>

<style>
.main_cont1{
    padding: 2px;
    width: 100%;
}
.middle_{
    width: 100%;
    display: flex;
    height: auto;
    flex-wrap: wrap;
    padding: 20px;
}
.circles_{
    display: flex;
    flex-wrap: wrap;
    width: 47%;
    justify-content: space-around;
}
.circle_1{
    padding: 10px;
}
.diagram_1{
    padding: 10px;
    width: 100%;
}
.diagram_{
    display: flex;
    margin-top: 20px;
    justify-content: space-around;
}
.diagram_img{
    width: 100%;
    height: auto;
}
.middle_value{
    margin-top: 20px;
}
.items_{
    display: flex;
    justify-content: space-between; 
    margin-top: 40px;
}
.circle_1_bar_1{
    display: flex;
    justify-content: space-between; 
}
.img__{
    margin: auto 0 auto 0 ;
}
  @media (max-width: 1200px) {
    .circle_1_bar_1{
        margin: auto;
    } 
    .middle_{
        
        justify-content: center;
    }
    .circles_{
        width: auto;
        justify-content: center;
    }
}
</style>
