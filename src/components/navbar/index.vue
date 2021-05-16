<template>
  <ul class="nav-bar">

    <li>
      <i class="icon icon-help"></i>
    </li>
    <li>
      <i class="icon icon-search"></i>
    </li>
    <li>
      <a href="javscript:;" class="select-cars">选择车辆</a>
    </li>
    <li>
      <i class="icon icon-location"></i>
    </li>
    <li>
      <i class="icon icon-user"></i>
    </li>

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
    .icon {
      margin: 0 17px;
      background-color: $main-color;
      border-radius: 50%;
      vertical-align: middle;
      cursor: pointer;
    }
    .select-cars {
      display: block;
      width: 240px;
      height: 84px;
      margin: 0 17px;
      border-radius: 100px;
      line-height: 84px;
      text-align: center;
      color: #fff;
      font-size: 26px;
      font-weight: 300;
      background-color: $main-color;
    }
  }
}
</style>