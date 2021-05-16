<template>
  <div class="amap-wrapper">
    <el-amap class="amap-box" :vid="'amapContainer'" :zoom="zoom"></el-amap>
  </div>
</template>

<script>
  import {
    lazyAMapApiLoaderInstance
  } from 'vue-amap';
  export default {
    name: 'cars',
    data() {
      return {
        map: null,
        zoom: 13
      }
    },
    mounted() {
      lazyAMapApiLoaderInstance.load().then(() => {
        this.map = new AMap.Map('amapContainer', {
          center: [116.403608, 39.907123],
          zoom: this.zoom
        });
      });
    },
  }
</script>

<style lang="scss" scoped>
  .amap-wrapper {
    height: 100vh;
  }
</style>