<template>
  <div>
    <Map />
    <Cars />
    <div class="user-wrapper" :class="{open: isOpen}">
      <router-view />
    </div>
    <nav-bar/>

  </div>
</template>

<script>
import Map from '../map';
import Cars from '../cars';
import NavBar from '@c/navbar'
export default {
  name: 'index',
  components: {
    Map,
    Cars,
    NavBar
  },
  data () {
    return {}
  },

  mounted () {

  },
  computed: {
    isOpen () {
      return this.$route.name === 'user' ? true : false
    }
  },
  watch: {}
}
</script>

<style lang="scss" scoped>
.user-wrapper {
  position: fixed;
  bottom: 0;
  right: -600px;
  width: 410px;
  height: 100%;
  background-color: #34393f;
  z-index: 101;
  transition: all 0.5s ease;

  &.open {
    right: 0;
  }
}
</style>