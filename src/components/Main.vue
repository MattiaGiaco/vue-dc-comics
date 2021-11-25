<template>
  <main>
    <div class="junbotron">
      
    </div>

    <div class="current-series">
      <div class="container">
        <SeriesCard 
        v-for="(product, index) in thumbData"  
        :key="index"
        :product="product"
        />
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
  main .junbotron{
    width: 100%;
    height: 400px;
    background-image: url(../assets/img/jumbotron.jpg);
  }

  main .current-series{
    min-height: 300px;
    background-color: #1c1c1c;
  }
</style>