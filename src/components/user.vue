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
        <div class="info">
          <div class="info-cat">出生年月</div>
          <div class="info-detail">1992年02月14日</div>
        </div>
        <div class="info">
          <div class="info-cat">籍贯</div>
          <div class="info-detail">汉族</div>
        </div>
        <div class="info">
          <div class="info-cat">婚姻状况</div>
          <div class="info-detail">未婚</div>
        </div>
        <div class="info">
          <div class="info-cat">手机</div>
          <div class="info-detail">18906702695</div>
        </div>
        <div class="info">
          <div class="info-cat">邮箱</div>
          <div class="info-detail">18906702695@163.com</div>
        </div>
        <div class="info">
          <div class="info-cat">户口</div>
          <div class="info-detail">江西省宜春市</div>
        </div>
        <div class="info">
          <div class="info-cat">状态</div>
          <div class="info-detail">离职,正在找工作</div>
        </div>
        <!--<mycell></mycell>-->
        <!--<div id="ability_echarts" style="width: 300px;height:300px;"></div>-->
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
    //import {Echarts} from '../assets/lib/echarts.min.js'
    let echarts = require('../assets/lib/echarts.min.js');
    //import MyCell from "components/mycell"
    export default {
        name: 'user',
        components: {
            Card,
            Divider,
            Group,
            Cell
        },
        data() {
            return {
                msg: 'Welcome to Your Vue.js App'
            }
        },
        beforeCreate: function(){
          console.log("beforeCreate ")
          console.log(echarts.echarts)
          console.log(document.getElementById('ability_echarts'))
          //var myChart = echarts.echarts.init(document.getElementById('ability_echarts'));
          var option = {
                  title: {
                      text: '黄彬的前端能力图'
                  },
                  tooltip: {},
                  legend: {
                      data: ['黄彬']
                  },
                  radar: {
                      // shape: 'circle',
                      indicator: [
                        { name: 'vuejs', max: 100},
                        { name: 'jquery', max: 100},
                        { name: 'javascript', max: 100},
                        { name: 'React', max: 100},
                        { name: '微信小程序', max: 100},
                        { name: '整体', max: 100}
                      ],
                      radius: 100
                  },
                  series: [{
                      name: '预算 vs 开销（Budget vs spending）',
                      type: 'radar',
                      // areaStyle: {normal: {}},
                      data : [
                          {
                              value : [80, 100, 95, 40, 50, 90],
                              name : '黄彬'
                          }
                      ]
                  }]
              }
          // 使用刚指定的配置项和数据显示图表。
         //myChart.setOption(option);
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

    .info {
        display: flex;
        flex-direction: row;
    }
    
    .info-cat {
        flex: 1;
        color: #999999;
        font-size: 16px;
    }
    
    .info-detail {
        flex: 1;
        text-align: right;
    }
</style>