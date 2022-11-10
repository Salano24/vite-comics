
<script>
import SiteHeader from "./components/SiteHeader.vue";
import SiteJumbo from "./components/SiteJumbo.vue";
import SiteMainNav from "./components/SiteMainNav.vue";
import SiteMain from "./components/SiteMain.vue";
import SiteFooter from "./components/SiteFooter.vue";


export default{
  name: 'App',
  components: {
   SiteHeader,
   SiteJumbo,
   SiteMainNav,
   SiteMain,
   SiteFooter
  }
}
</script>

<template>
  <site-header></site-header>

  <site-jumbo></site-jumbo>

  <site-main-nav></site-main-nav>

  <site-main></site-main>

  <footer>
    <div class="container">
      <div class="signUp"><button>SIGN-UP NOW!</button></div>
      <div class="social">
        <span>FOLLOW US</span>
        <img src="./assets/img/footer-facebook.png" alt="">
        <img src="./assets/img/footer-twitter.png" alt="">
        <img src="./assets/img/footer-youtube.png" alt="">
        <img src="./assets/img/footer-pinterest.png" alt="">
        <img src="./assets/img/footer-periscope.png" alt="">

      </div>
    </div>
  </footer>
</template>

<style scoped lang="scss">
  
</style>