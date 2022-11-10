<script>
export default{
    name: 'SiteMain',
    data() {
      return {
        shop:[
          {
            text: 'DC COMICS',
            links: [
              'Characters',
              'Comics',
              'Movies',
              'TV',
              'Games',
              'Videos',
              'News'
            ]
          },
          {
            text: 'DC',
            links: [
              'Characters',
              'Comics',
              'Movies',
              'TV',
              'Games',
              'Videos',
              'Characters',
              'Comics',
              'Movies',
              'TV',
              'Games',
              'Videos',
              
            ]
          },
          {
            text: 'DC COMICS',
            links: [
              'DC',
              'MAD Magazine',
              'DC Kids',
              'DC Universe',
              'DC Power Visa',
              
            ]
          },
          {
            text: 'SHOP',
            links: [
              'Shop DC',
              'Shop DC Collectables',
              
            ]
          }
        ]
      }
    }
}
</script>

<template>
      <main>
    <div class="container d-flex">
      <div class="mainText">
        <div class="container">
          <div class="row">
            <div class="col-4" v-for="item in shop">
              <h3>{{item.text}}</h3>
              <span v-for="link in item.links">{{link}}</span>
            </div>
          
          </div>
        </div>
      </div>
      <div class="mainImg">
        <img src="../assets/img/dc-logo-bg.png" alt="">
      </div>
    </div>
  </main>
</template>