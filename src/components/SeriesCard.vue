<template>
  <div class="card">
    <img :src="product.thumb" :alt="product.series">
    <h3>{{product.series}}</h3>
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
    width: calc(100% / 6);
    height: 250px;
    margin: 30px 0;
    border: 20px solid #1c1c1c;
    img{
      width: 100%;
      height: 100%;
      margin-bottom: 10px;
      object-fit: cover;
    }
  }
</style>