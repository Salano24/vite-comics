<script>
export default{
    name: 'SiteHeader',
    data() {
      return {
        headerNav: [
          {
            text: CHARACTERS,
            active: false
          },
          {
            text: COMICS,
            active: true
          },
          {
            text: MOVIES,
            active: false
          },
          {
            text: TV,
            active: false
          },
          {
            text: GAMES,
            active: false
          },
          {
            text: COLLECTIBLES,
            active: false
          },
          {
            text: VIDEOS,
            active: false
          },
          {
            text: FANS,
            active: false
          },
          {
            text: NEWS,
            active: false
          },
          {
            text: SHOP,
            active: false
          },
        ]

        
      }
    }
}
</script>

<template>
  <header>
    <div class="container">
      <div class="logo">
        <img src="../assets/img/dc-logo.png" alt="">
      </div>
      <div class="header_nav">
       <a href="#" v-for="item in headerNav" :class="item.active === true ? 'active' : ''">{{item.text}}</a>
      </div>
    </div>
  </header>
</template>