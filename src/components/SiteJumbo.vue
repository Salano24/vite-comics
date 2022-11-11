<script>
import comics from '../dc-comics.js'
export default{

  props:{
    image: String,
    title: String
},
    name: 'SiteJumbo',
    data() {
      return {
        comics: comics
      }
    }
}
</script>

<template>
      <div class="jumbo"> 
        <div class="current">
         <img src="../assets/img/jumbotron.jpg" alt=""> 
        </div>
      <div class="container">
        <div class="row">
        <div class="col-2" v-for="comic in comics">
        <div class="comic">
            <img :src="comic.thumb" alt="">
            <h4>{{ comic.series }}</h4>
        </div>
      </div>
    </div> 
    <div class="load">
      <button>LOAD MORE</button>
    </div>
      </div>
    </div>
 
</template>