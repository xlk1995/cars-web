<template>
  <div class="cars-wrapper" @click="$router.push('/user')">
    汽车列表
  </div>
</template>

<script>
export default {
  name: 'cars'
}
</script>

<style lang="scss" scoped>
.cars-wrapper {
  position: fixed;
  top: 0;
  left: 0;
  z-index: 100;
}
</style>