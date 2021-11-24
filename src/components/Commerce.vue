<template>
  <div class="commerce">
    <div class="container">
      <div class="commerce-content">
        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
        <span>digital comics</span>
      </div>
      <div class="commerce-content">
        <img src="../assets/img/buy-comics-merchandise.png" alt="">
        <span>digital comics</span>
      </div>  
      <div class="commerce-content">
        <img src="../assets/img/buy-comics-shop-locator.png" alt="">
        <span>digital comics</span>
      </div>  
      <div class="commerce-content">
        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
        <span>digital comics</span>
      </div>  
      <div class="commerce-content">
        <img src="../assets/img/buy-dc-power-visa.svg" alt="">
        <span>digital comics</span>
      </div>  
    </div>
  </div>
</template>

<script>
export default {
  name: 'Commerce'
}
</script>

<style lang="scss">

@import "../assets/scss/var.scss";

  .commerce{
    background-color: $primaryColor;
  }
  .commerce .container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
    .commerce-content{
      display: flex;
      align-items: center;
      cursor: pointer;
      padding: 20px;
    }
    span{
      text-transform: uppercase;
      font-size: 12px;
    }
  }
  img{
    width: 40px;
    margin-right: 10px;
 }
</style>