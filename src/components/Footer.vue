<template>
  <footer>
    <div class="footer-top">
      <div class="container">
        <div class="info">
          <div class="footer-links">
            <h4>dc comics</h4>
            <ul>
              <li><a href="#">Characters</a></li>
              <li><a href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
              <li><a href="#">TV</a></li>
              <li><a href="#">Games</a></li>
              <li><a href="#">Videos</a></li>
              <li><a href="#">News</a></li>
            </ul>
            <h4>shop</h4>
            <ul>
              <li><a href="#">Shop DC</a></li>
              <li><a href="#">Shop DC Collectibles</a></li>
            </ul>
          </div>
          <div class="footer-links">
            <h4>dc</h4>
            <ul>
              <li><a href="#">Terms Of Use</a></li>
              <li><a href="#">Privacy policy(New)</a></li>
              <li><a href="#">Ad Choices</a></li>
              <li><a href="#">Advertising</a></li>
              <li><a href="#">Jobs</a></li>
              <li><a href="#">Subscription</a></li>
              <li><a href="#">Talent Workshop</a></li>
              <li><a href="#">CPSC Certificates</a></li>
              <li><a href="#">Ratings</a></li>
              <li><a href="#">Shop Help</a></li>
              <li><a href="#">Contact Us</a></li>
            </ul>
          </div>
          <div class="footer-links">
            <h4>sites</h4>
            <ul>
              <li><a href="#">DC</a></li>
              <li><a href="#">MAD Magazine</a></li>
              <li><a href="#">DC Kids</a></li>
              <li><a href="#">DC Universe</a></li>
              <li><a href="#">DC Power Visa</a></li>
            </ul>
          </div>
        </div>  
        <div class="logo-bg">
          <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>
      </div>
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
    background-image: url(../assets/img/footer-bg.jpg);
  }
  .footer-top .container{
    display: flex;
    justify-content: space-between;
    .info{
      display: flex;
    }
    .footer-links{
      padding: 30px 0;
      margin-right: 20px;
    }
    h4{
      margin: 10px 0;
      text-transform: uppercase;
    }
    ul li{
      line-height: 22px;
    }
    ul li a{
      color: #787878;
      &:hover{
        color: $primaryColor;
      }
    }
  }
  
  .logo-bg img{
  
  }

  .footer-bottom{
    background-color: #303030;
  }

  .footer-bottom .container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 80px;
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
      cursor: pointer;
    }
  }
</style>