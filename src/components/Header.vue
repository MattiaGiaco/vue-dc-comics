<template>
  <header class="container">
    <img src="../assets/img/dc-logo.png" alt="">
    <div class="menu">
      <ul>
        <li v-for="(item, index) in links" :key="index">
          <a :class="{active: item.current}" :href="item.url">{{item.text}}</a>
        </li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data(){
    return{
      links:[
        {
          url: '/characters',
          text: 'characters',
          current: false
        },
        {
          url: '/comics',
          text: 'comics',
          current: true
        },
        {
          url: '/movies',
          text: 'movies',
          current: false
        },
        {
          url: '/tv',
          text: 'tv',
          current: false
        },
        {
          url: '/games',
          text: 'games',
          current: false
        },
        {
          url: '/collectibles',
          text: 'collectibles',
          current: false
        },
        {
          url: '/videos',
          text: 'videos',
          current: false
        },
        {
          url: '/fans',
          text: 'fans',
          current: false
        },
        {
          url: '/news',
          text: 'news',
          current: false
        },
        {
          url: '/shop',
          text: 'shop',
          current: false
        }
      ]
    }
  }
}
</script>

<style lang="scss">

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
  img{
    width: 70px;
  }
</style>