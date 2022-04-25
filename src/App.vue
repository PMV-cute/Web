<template>
<div class="main_con">
  <div class="left_cont">
    <left></left>
  </div>
<div class="cont">
  <div class="top_cont">
    <top></top>
  </div>
  <div class="top_cont">
    <middle></middle>
  </div>
  <div class="top_cont">
    <bottom></bottom>
  </div>
</div>
</div>


</template>

<script lang="ts">
import top from './components/top_bar.vue'
import middle from './components/middle_bar.vue'
import bottom from './components/bottom_bar.vue'
import left from './components/left_menu.vue'
export default ({
  name: 'App',
  components: {
    top,
    middle,
    bottom,
    left
  }
});
</script>

<style>
.main_con{
  width: 100%;
  margin: 0 auto;
  display: flex;
  flex-direction: row;

}
.left_cont{
  display: flex;
  flex-basis: 250px;
  margin: 0 auto 0 0;
}
.cont{
  width: 100%;
}
.top_cont{
  display: flex;
  width: 100%;
  justify-content: center;
}
body{
  padding: -8px;
}
 @media (max-width: 1200px) {
    .left_cont{
      flex-basis: 70px;
    }
}
</style>
