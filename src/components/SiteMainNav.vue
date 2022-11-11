<script>
export default{
    name: 'SiteHeader',
    data() {
      return {
        mainNav: [
          {
            text: 'DIGITAL COMICS',
            fonte: "buy-comics-digital-comics.png"
          },
          {
            text: 'DC MERCHANDISE',
            fonte: 'buy-comics-merchandise.png'
          },
          {
            text: 'SUBSCRIPTION',
            fonte: 'buy-comics-subscriptions.png'
          },
          {
            text: 'COMIC SHOP LOCATOR',
            fonte: 'buy-comics-shop-locator.png'
          },
          {
            text: 'DC POWER VISA',
            fonte: 'buy-dc-power-visa.svg'
          },
          
        ]
       

      }
    },
    methods:{
       getImageUrl(fonte) {
  return new URL(`../assets/img/${fonte}`, import.meta.url).href
}

    }
}
</script>

<template>
 <div class="mainnav">
    <div class="container">
      <div class="navItem" v-for="item in mainNav">
        <img :src="getImageUrl(item.fonte)" alt="">
        <span>{{item.text}}</span>
      </div>
     
    </div>
  </div>
</template>