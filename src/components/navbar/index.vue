<template>
  <ul class="nav-bar">

    <li>1</li>
    <li>1</li>
    <li>1</li>
    <li>1</li>

  </ul>
</template>

<script>
export default {
  name: 'navbar',
  data () {
    return {
    }
  },
}
</script>

<style lang="scss" scoped>
.nav-bar {
  z-index: 10;
  position: fixed;
  left: 0;
  right: 0;
  bottom: 86px;
  text-align: center;
  li {
    display: inline-block;
  }
}
</style>