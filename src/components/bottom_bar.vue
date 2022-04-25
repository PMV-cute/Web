<template>
  <div class="main_cont2">
      <div class="bottom_">
          <div class="calendar_">
              <div class="calendar_1">
                  <img src="../assets/bottom_bar/Date-picker.png" alt="" class="img_auto">
              </div>
              
          </div>
          <div class="data_">
            <div class="bottom_bar">
                <img src="../assets/bottom_bar/Orders.png" alt="1" class="img_bar">
                <div class="bottom_bar_right">
                    <img src="../assets/bottom_bar/Medium2.png" alt="2" class="img_bar" style="cursor: pointer;">
                    <img src="../assets/bottom_bar/Medium1.png" alt="2" class="img_bar" style="cursor: pointer;">
                    <img src="../assets/bottom_bar/Medium.png" alt="2" class="img_bar" style="cursor: pointer;">
                </div>
                
            </div>
            <div class="table_">
                <img src="../assets/bottom_bar/Table.png" alt="" class="img_auto">
            </div>
              
          </div>
      </div>
  </div>

</template>

<script lang="ts">

</script>

<style>
.main_cont2{
    padding: 2px;
    width: 100%;
}
.bottom_{
    width: 100%;
    display: flex;
    height: auto;
    flex-wrap: wrap;
    padding: 0px;
}
.calendar_{
    width: 35%;
    display: flex;
    justify-content: space-around;
    margin-top: 30px;
}
.calendar_1{
    width: 75%;
}
.data_{
    flex-wrap: wrap;
    width: 60%;
    margin-top: 30px;
}
.img_auto{
    width: 100%;
    height: auto;
}
.bottom_bar{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between; 
}
.bottom_bar_right{
    display: flex;
}
.img_bar{
    margin: auto 0 auto 10px;
}
.table_{
    display: flex;
    justify-content:space-around;
    margin-top: 20px;
}
  @media (max-width: 1200px) {
    .data_ ,.calendar_{
        width: auto;
        justify-content: center;
    }
    .bottom_{
        justify-content: center;
    }
}
</style>
