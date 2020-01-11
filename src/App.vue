<template>
  <div id="app">
    <h1>屌毛表情包之年终大赏</h1>
    <div class="swiper-container">
        <div class="swiper-wrapper">
           <div class="swiper-slide"><img src="./assets/1.png" alt=""></div>
           <div class="swiper-slide"><img src="./assets/2.gif" alt=""></div>
           <div class="swiper-slide"><img src="./assets/3.jpg" alt=""></div>
           <div class="swiper-slide"><img src="./assets/4.jpg" alt=""></div>
           <div class="swiper-slide"><img src="./assets/5.jpg" alt=""></div>
           <div class="swiper-slide"><img src="./assets/6.gif" alt=""></div>
           <div class="swiper-slide"><img src="./assets/7.jpg" alt=""></div>
           <div class="swiper-slide"><img src="./assets/8.jpg" alt=""></div>
           <div class="swiper-slide"><img src="./assets/9.jpg" alt=""></div>

        </div>
    </div>
  </div>
</template>

<script>
import Swiper from 'swiper';
import 'swiper/css/swiper.min.css';

export default {
  name: 'app',
  components: {
    
  },
  data(){
    return{
      
    }
  },
  methods:{
    get(app){
      console.log(1111)
    }
  },
  mounted(){
    let mySwiper = new Swiper('.swiper-container', {
      effect : 'cube',
      loop: true,
      autoplay: {
          delay: 2000,
          disableOnInteraction: false,
      },
    })
    this.get(mySwiper)
  }
}
</script>

<style>
body{
  background: #333
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #fff;
  margin-top: 60px;
}
.swiper-container {
  width: 600px;
  height: 450px;
}
img{
  width: 100%;
  height: 100%
}
h1{
  text-align: center
}
</style>
