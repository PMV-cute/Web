<template>
 <iframe :srcdoc="result" class="frame" id="frame"></iframe>
</template>

<script lang="ts">
    export default {
    props: {
      result: [],
    },
  };
</script>

<style>
.frame {
  width: 100%;
  height: 2000px;
}
</style>