<script>
export default{
    name: 'SiteHeader',
    data() {
      return {
        mainNav: [
          {
            text: 'DIGITAL COMICS',
            fonte: "../assets/img/buy-comics-digital-comics.png"
          },
          {
            text: 'DC MERCHANDISE',
            fonte: '../assets/img/buy-comics-merchandise.png'
          },
          {
            text: 'SUBSCRIPTION',
            fonte: '../assets/img/buy-comics-subscriptions.png'
          },
          {
            text: 'COMIC SHOP LOCATOR',
            fonte: '../assets/img/buy-comics-shop-locator.png'
          },
          {
            text: 'DC POWER VISA',
            fonte: '../assets/img/buy-dc-power-visa.svg'
          },
          
        ]
       

      }
    }
}
</script>

<template>
 <div class="mainnav">
    <div class="container">
      <div class="navItem" v-for="item in mainNav">
        <img :src="item.fonte" alt="">
        <span>{{item.text}}</span>
      </div>
     
    </div>
  </div>
</template>