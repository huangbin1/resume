<template>
  <div class="user">
    <div class="photo">
      <img src="../assets/huangbin.png"></img>
    </div>
    <card :header="{title:'基本资料'}">
      <p slot="content" class="card-padding">出生年份 手机 户口 等</p>
    </card>
    <card :header="{title:'职业意向'}">
      <p slot="content" class="card-padding">前端开发工程师</p>
    </card>
    <card :header="{title:'工作经历'}">
      <p slot="content" class="card-padding">上海华测导航技术股份有限公司</p>
    </card>
    <card :header="{title:'教育经历'}">
      <p slot="content" class="card-padding">杭州电子科技大学</p>
    </card>
    <card :header="{title:'自我评价'}">
      <p slot="content" class="card-padding">很美很温柔！</p>
    </card>
    <card :header="{title:'附加信息'}">
      <p slot="content" class="card-padding">喜欢打人</p>
    </card>
    <card :header="{title:'擅长技能'}">
      <p slot="content" class="card-padding">vue</p>
    </card>
  </div>
</template>

<script>
    import {
        Card,
        Divider
    } from 'vux'
    export default {
        name: 'user',
        components: {
            Card,
            Divider
        },
        data() {
            return {
                msg: 'Welcome to Your Vue.js App'
            }
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .user {
        width: 100%;
        bottom: 55px;
        top: 0px;
    }
    
    .photo {
        margin: 0 auto;
        width: 120px;
        height: 120px;
    }
    
    .card-padding {
        padding: 15px;
    }
</style>