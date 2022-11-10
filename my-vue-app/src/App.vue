
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
</template>

<style scoped lang="scss">

</style>