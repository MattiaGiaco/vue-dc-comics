<template>
  <header class="container">
    <img src="../assets/img/dc-logo.png" alt="">
    <div class="menu">
      <ul>
        <li v-for="(item, index) in menuData" :key="index">
          <a :class="{active: item.current}" :href="item.url">{{item.text}}</a>
        </li>
      </ul>
    </div>
  </header>
</template>

<script>

import menuData from '../assets/data/menuData.js';

export default {
  name: 'Header',
  data(){
    return{
      menuData,
    }
  }
}
</script>

<style lang="scss" scoped>

@import "../assets/scss/var.scss";

  header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100px;
    ul{
      display: flex;
    }
    li a{
      padding: 37px 10px;
      font-size: 12px;
      font-weight: bold;
      color: black;
      text-transform: uppercase;
      &:hover,
      &.active {
        color: $primaryColor;
        border-bottom: 5px solid $primaryColor;
      }
    }
  }
  header img{
    width: 70px;
  }
</style>