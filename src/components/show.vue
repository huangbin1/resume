<template>
  <div class="show">
   <divider>pc page</divider>
   <swiper auto height="300px">
      <swiper-item class="black"> <img src="../assets/i80NewImage/1.png" class="imgSize"></img></swiper-item>
      <swiper-item class="black"> <img src="../assets/i80NewImage/2.png" class="imgSize"></img></swiper-item>
      <swiper-item class="black"> <img src="../assets/i80NewImage/3.png" class="imgSize"></img></swiper-item>
      <swiper-item class="black"> <img src="../assets/i80NewImage/4.png" class="imgSize"></img></swiper-item>
      <swiper-item class="black"> <img src="../assets/i80NewImage/5.png" class="imgSize"></img></swiper-item>
      <swiper-item class="black"> <img src="../assets/i80NewImage/6.png" class="imgSize"></img></swiper-item>
      <swiper-item class="black"> <img src="../assets/i80NewImage/7.png" class="imgSize"></img></swiper-item>
      <swiper-item class="black"> <img src="../assets/i80NewImage/8.png" class="imgSize"></img></swiper-item>
      <swiper-item class="black"> <img src="../assets/i80NewImage/9.png" class="imgSize"></img></swiper-item>
    </swiper>
    <divider>mobile page</divider>
    <swiper auto height="500px">
      <swiper-item class="black"> <img src="../assets/i80MobileImage/1.png" class="imgSize"></img></swiper-item>
      <swiper-item class="black"> <img src="../assets/i80MobileImage/2.png" class="imgSize"></img></swiper-item>
      <swiper-item class="black"> <img src="../assets/i80MobileImage/3.png" class="imgSize"></img></swiper-item>
      <swiper-item class="black"> <img src="../assets/i80MobileImage/4.png" class="imgSize"></img></swiper-item>
      <swiper-item class="black"> <img src="../assets/i80MobileImage/5.png" class="imgSize"></img></swiper-item>
      <swiper-item class="black"> <img src="../assets/i80MobileImage/6.png" class="imgSize"></img></swiper-item>
      <swiper-item class="black"> <img src="../assets/i80MobileImage/7.png" class="imgSize"></img></swiper-item>
    </swiper>
    <divider>pc page</divider>
    <swiper auto height="300px">
      <swiper-item class="black"> <img src="../assets/i80MobileImage/1.png" class="imgSize"></img></swiper-item>
      <swiper-item class="black"> <img src="../assets/i80MobileImage/2.png" class="imgSize"></img></swiper-item>
      <swiper-item class="black"> <img src="../assets/i80MobileImage/3.png" class="imgSize"></img></swiper-item>
      <swiper-item class="black"> <img src="../assets/i80MobileImage/4.png" class="imgSize"></img></swiper-item>
      <swiper-item class="black"> <img src="../assets/i80MobileImage/5.png" class="imgSize"></img></swiper-item>
      <swiper-item class="black"> <img src="../assets/i80MobileImage/6.png" class="imgSize"></img></swiper-item>
      
    </swiper>
  </div>
</template>

<script>
    import {
       Swiper,
    SwiperItem,
    GroupTitle,
    XButton,
    Divider
    } from 'vux'
    //import {Echarts} from '../assets/lib/echarts.min.js'
   
    //import MyCell from "components/mycell"
    export default {
        name: 'show',
        components: {
            Swiper,
    SwiperItem,
    GroupTitle,
    XButton,
    Divider
        },
        data() {
            return {
                msg: 'Welcome to Your Vue.js App'
            }
        },
   
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
   .imgSize{
   width:100%;
   height:100%;
   }
</style>