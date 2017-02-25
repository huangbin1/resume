<template>
  <div class="user">
    <div class="photo">
      <img src="../assets/huangbin.png"></img>
      <div class="photo-info">
        <div class="photo-name">
          <h3>黄彬</h3>&nbsp&nbsp女
        </div>
        <div class="photo-job">
          目前职位：web前端工程师
        </div>
        <div class="photo-age">
          工作年限：2年以上
        </div>
      </div>
    </div>
    <card :header="{title:'基本资料'}">
      <div slot="content" class="card-padding">
        <mycell></mycell>
      </div>
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
        Divider,
        Group,
        Cell
    } from 'vux'
    import MyCell from "components/mycell"
    export default {
        name: 'user',
        components: {
            Card,
            Divider,
            Group,
            Cell,
            MyCell
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
        display: flex;
        flex-direction: row;
    }
    
    .photo img {
        display: block;
        padding: 10px 10px 0 20px;
        width: 120px;
        height: 120px;
    }
    
    .photo-name h3 {
        color: #128811;
        display: inline;
    }
    
    .photo-info {
        flex: 1;
    }
    
    .photo-info div {
        padding: 8px;
    }
    
    .card-padding {
        padding: 15px;
    }
</style>