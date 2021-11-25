<template>
  <div class="card">
    <img :src="product.thumb" alt="">
    <h3></h3>
  </div>
</template>

<script>
export default {
  name: 'thumbData',
  props:{
    product: Object,
  }
}
</script>

<style lang="scss" scoped>
  .card{
    width: 200px;
    height: 200px;
  }
</style>