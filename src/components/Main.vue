<template>
  <main>
    <div class="junbotron">
      
    </div>

    <div class="current-series">
      <div class="title">
        current series
      </div>
      <div class="container box">
        <SeriesCard 
        v-for="(product, index) in thumbData"  
        :key="index"
        :product="product"
        />
      </div>

      <div class="button">
        <button>load more</button>
      </div>
    </div>
  </main>
</template>

<script>

import SeriesCard from './SeriesCard';
import thumbData from '../assets/data/thumbData.js';

export default {
  name: 'Main',
  components:{
    SeriesCard
  },
  data(){
    return{
      thumbData,
    }
  }
}
</script>

<style lang="scss" scoped>

@import "../assets/scss/var.scss";

  main .junbotron{
    width: 100%;
    height: 400px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
  }

  main .current-series{
    position: relative;
    min-height: 300px;
    background-color: #1c1c1c;
    .box{
      display: flex;
      flex-wrap: wrap;
      padding-bottom: 80px;
    }   
  }
  .button{
    display: flex;
    justify-content: center;
    padding-bottom: 20px;
    button{
      padding: 10px 50px;
      background-color: $primaryColor;
      border: none;
      color: white;
      text-transform: uppercase;
      font-weight: bold;
    }
  }

  .title{
    position: absolute;
    top: -30px;
    left: 20%;
    background-color: $primaryColor;
    width: 18%;
    text-align: center;
    padding: 20px;
    color: white;
    text-transform: uppercase;
    font-weight: bold;
    font-size: 25px;
  }
      </style>