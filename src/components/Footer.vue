<template>
  <footer>
    <div class="footer-top">

    </div>

    <div class="footer-bottom">
      <div class="container">
        <button>sign-up now!</button>
        <div class="social">
          <span>follow us</span>
          <img src="../assets/img/footer-facebook.png" alt="">
          <img src="../assets/img/footer-twitter.png" alt="">
          <img src="../assets/img/footer-youtube.png" alt="">
          <img src="../assets/img/footer-pinterest.png" alt="">
          <img src="../assets/img/footer-periscope.png" alt="">
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style lang="scss">

@import "../assets/scss/var.scss";

  .footer-top{
    min-height: 300px;
    background-image: url(../assets/img/footer-bg.jpg);
  }

  .footer-bottom{
    background-color: #303030;
  }

  .footer-bottom .container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 30px 0;
    button{
      padding: 10px;
      background-color: transparent;
      border: 2px solid $primaryColor;
      color: white;
      text-transform: uppercase;
      font-weight: bold;
      cursor: pointer;
    }
  }
  .footer-bottom .social{
    display: flex;
    align-items: center;
    span{
      text-transform: uppercase;
      color: $primaryColor;
      font-weight: bold;
      margin-right: 15px;
    }
    img{
      width: 30px;
      margin-left: 10px;
    }
  }
</style>