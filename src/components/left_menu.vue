<template>
  <div class="main_cont3">
      <div class="left_">
          <div class="left_menu">
              <div class="li">
                  <img src="../assets/left_menu/email-png-icon-free-download-732604.png" alt="" class="img_auto1">
                <p>Messages</p>
                </div>
              <div class="li">
                  <img src="../assets/left_menu/123.png" alt="" class="img_auto1">
                <p>Discover</p>
                </div>
                <div class="li">
                  <img src="../assets/left_menu/8d7ca49add3c477989d0b490041e378b.jpg" alt="" class="img_auto1">
                <p>Call</p>
                </div>
                <div class="li">
                  <img src="../assets/left_menu/pngtree-info-vector-icon-png-image_470297.png" alt="" class="img_auto1">
                <p>Info</p>
                </div>
          </div>
          
      </div>
  </div>

</template>

<script lang="ts">

</script>

<style>
.main_cont3{
    padding: 2px;
    width: 100%;
    background-color: rgb(194, 192, 192);
}
.left_{
    width: 100%;
    display: flex;
    height: auto;
    flex-wrap: wrap;
    padding: 0px;
    justify-content: center;
}
.left_menu{
    display: flex;
     flex-direction: column;
     margin-top: 100px;
}
.img_auto1{
    width: 20px;
    height: 20px;
    margin: auto 0;
}
.li{
    display: flex;
    height: 50px;
}
p {
    margin: auto 0 auto 20px;
    
}
  @media (max-width: 1200px) {
    p {
        display: none;
    }
}
</style>
