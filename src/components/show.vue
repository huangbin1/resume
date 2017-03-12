<template>
  <div class="show">
   <divider>pc page</divider>
   <swiper auto height="210px">
      <swiper-item class="black"> <img src="../assets/i80NewImage/1.png" class="imgSize"></img></swiper-item>
      <swiper-item class="black"> <img src="../assets/i80NewImage/2.png" class="imgSize"></img></swiper-item>
      <swiper-item class="black"> <img src="../assets/i80NewImage/3.png" class="imgSize"></img></swiper-item>
    </swiper>
    <divider>mobile page</divider>
    <swiper auto height="600px">
      <swiper-item class="black"> <img src="../assets/i80MobileImage/1.jpg" class="imgSize"></img></swiper-item>
      <swiper-item class="black"> <img src="../assets/i80MobileImage/2.png" class="imgSize"></img></swiper-item>
      <swiper-item class="black"> <img src="../assets/i80MobileImage/3.png" class="imgSize"></img></swiper-item>
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
   .show{
       padding-bottom:3.2rem;
   }
</style>