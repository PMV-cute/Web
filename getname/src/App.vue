<template>
    <div id="app">
      <FIO/>
      
      <Vyatsu :results="results"></Vyatsu>
      <LogPas></LogPas>
    </div>
</template>

<script lang="ts">

import Vyatsu from '../../vyatsu/src/components/Vyatsu_F.vue'
import FIO from '../../fio/src/components/FIO.vue'
import LogPas from '../../logpas/src/components/LogPas.vue'

import axios from 'axios';
import {defineComponent} from 'vue';
  const config = {
    headers: {
      'Access-Control-Allow-Origin': 'https://yandex.ru/news',
    },
  };

  const url = 'https://yandex.ru/news';
export default defineComponent({
name: 'App',
components: {FIO, LogPas, Vyatsu},
data(){
  return{
      result:[]
      };
    },
    mounted(){
      axios
      .get(url,
      { headers: {"Access-Control-Allow-Origin" : "https://yandex.ru/news" },
      withCredentials: false,}
    ).then((response: any) =>
        {this.result = response.data;},
        ); 
  }, 
  });

</script>
<style>

</style>