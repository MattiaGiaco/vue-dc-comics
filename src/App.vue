<template>
  <div>
    <Header />
    <Main />
    <Commerce />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue"
import Main from "./components/Main.vue"
import Commerce from "./components/Commerce.vue"
import Footer from "./components/Footer.vue"

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Commerce,
    Footer
  }
}
</script>

<style lang="scss">
@import './assets/scss/common.scss';
@import './assets/scss/var.scss';
@import './assets/scss/utilities.scss';

</style>
