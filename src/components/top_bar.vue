<template>
  <div class="main_cont">
      <div class="top_">
        <div class="top_left">
          <img src="../assets/Logo.png" alt="logo" class="img_">
          <img src="../assets/Card2.png" alt="name_comp" class="img_">
        </div>
        <div class="top_right">
            <input placeholder="Search" class="input" type="text"/>
            <img src="../assets/icon.png" alt="icon1_top" class="img_" style="cursor: pointer;">
            <img src="../assets/Medium.png" alt="icon2_top" class="img_" style="cursor: pointer;">
        </div>
      </div>
    <div class="top_">
        <div class="top_left_b">
          <img src="../assets/top_bottom/Dashboard.png" alt="logo" class="img_" style="cursor: pointer;">
          <img src="../assets/top_bottom/Inbox.png" alt="name_comp" class="img_" style="cursor: pointer;">
          <img src="../assets/top_bottom/Security.png" alt="name_comp" class="img_" style="cursor: pointer;">
          <img src="../assets/top_bottom/Calendar.png" alt="name_comp" class="img_" style="cursor: pointer;">
          <img src="../assets/top_bottom/more-horizontal.png" alt="name_comp" class="img_" style="cursor: pointer;">
        </div>
        <div class="top_right_b">
            <img src="../assets/top_bottom/28.png" alt="name_comp" class="img_">
        </div>
    </div>
  </div>

</template>

<script lang="ts">

</script>

<style>
.main_cont{
    padding: 2px;
    width: 100%;
}
.top_{
    display: flex;
    flex: row;
    flex-wrap: wrap;
    align-content: center;
    height: auto;
}
.top_left{
    display: flex;
    height: 80px;
    margin-right: auto;
}
.top_right{
      display: flex;
    height: 80px;
    margin-left: auto;
}
.top_left_b{
    display: flex;
    height: 50px;
    margin-right: auto;
}
.top_right_b{
    display: flex;
    height: 50px;
    margin-left: auto;
}
.img_{
    padding: 10px;
    margin: auto 0 auto 0;
    
}

.input {
    max-width: 200px;
    height: 20%;
    color: rgb(0, 0, 0);
    border: 0;
    border-radius: 5px;
    box-shadow: inset 0 1px 4px rgba(0, 0, 0, 0.3), 0 1px rgba(255, 255, 255, 0.06);
    padding: 10px;
    margin: auto 0 auto 0;
  }
  @media (max-width: 1200px) {
    .top_left_b{
        margin: auto;
    } 
    .top_right_b {
        margin: auto;
    }
    .top_left{
        margin: auto;
    }
    .top_right{
        margin: auto;
    }
}
</style>
