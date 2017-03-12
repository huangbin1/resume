<template>
  <div class="user">
    <div class="photo">
      <img src="../assets/huangbin.png"></img>
      <div class="photo-info">
          <p>黄彬</p>
          <p>求职意向：前端工程师</p>
          <p>工作年限：2年</p>
      </div>
    </div>
    <div>
        <div class="contact">
            <a href="https://www.zhihu.com/people/xiaxiaowen-68"><img src="../assets/contactImage/zhihu.png"></img></a>
            <a href="http://weibo.com/2624719700/profile?topnav=1&wvr=6"><img src="../assets/contactImage/weibo.png"></img></a>
            <a href="https://sns.liepin.com/main/5674995339j3099828089"><img src="../assets/contactImage/lieping.png"></img></a>
            <a href="https://github.com/huangbin1"><img src="../assets/contactImage/QQ.png"></img></a>
            <a href="https://github.com/huangbin1"><img src="../assets/contactImage/wechart.png"></img></a>
            <a href="https://github.com/huangbin1"><img src="../assets/contactImage/github.png"></img></a>
        </div>
    </div>
    <div id="mychart" style="width:18rem;height:18rem;" ref="mychart"></div>
    <card :header="{title:'基本资料'}">
      <div slot="content" class="card-padding">
        <div class="info">
          <div class="info-cat">出生年月</div>
          <div class="info-detail">1992/12/26</div>
        </div>
        <div class="info">
          <div class="info-cat">籍贯</div>
          <div class="info-detail">江西省高安市</div>
        </div>
        <div class="info">
          <div class="info-cat">学历</div>
          <div class="info-detail">本科11级</div>
        </div>
        <div class="info">
          <div class="info-cat">毕业时间</div>
          <div class="info-detail">2015/06/30</div>
        </div>
        <div class="info">
          <div class="info-cat">毕业学校</div>
          <div class="info-detail">杭州电子科技大学</div>
        </div>
        
        <div class="info">
          <div class="info-cat">专业</div>
          <div class="info-detail">电子信息工程</div>
        </div>
        <div class="info">
          <div class="info-cat">联系电话</div>
          <div class="info-detail">18906702695</div>
        </div>
        <div class="info">
          <div class="info-cat">邮箱</div>
          <div class="info-detail">18906702695@163.com</div>
        </div>
        <div class="info">
          <div class="info-cat">状态</div>
          <div class="info-detail">离职,正在找工作</div>
        </div>
        <!--<mycell></mycell>-->
      </div>
    </card>
    <card :header="{title:'求职意向'}">
      <div slot="content" class="card-padding">
        <div class="info">
        <div class="info-cat">目标职位</div>
        <div class="info-detail" style="flex:2">前端工程师</div>
        </div>
      </div>
    </card>
    <card :header="{title:'工作经历'}">
      <div slot="content" class="card-padding">
        <div class="info">
          <div class="info-cat">2015.3-2017.3</div>
          <div class="info-detail" style="flex:2">上海华测导航技术股份有限公司</div>
        </div>
      </div>
    </card>
    <card :header="{title:'教育经历'}">
      <div slot="content" class="card-padding">
        <div class="info">
          <div class="info-cat">2011.9-2015.6</div>
          <div class="info-detail" style="flex:2">杭州电子科技大学</div>
        </div>
        <div class="info">
          <div class="info-cat">英语</div>
          <div class="info-detail" style="flex:2">CET-6</div>
        </div>
        <div class="info">
          <div class="info-cat">计算机</div>
          <div class="info-detail" style="flex:2">计算机二级C</div>
        </div>
      </div>
    </card>
    <card :header="{title:'自我评价'}">
      <div slot="content" class="card-padding">
        <div class="info">
          1活泼好动，积极主动
        </div>
        <div class="info">
          2有强烈的上进心和求知欲，善于学习和运用新知识，很喜欢前端
        </div>
      </div>
    </card>
    <card :header="{title:'专业技能'}">
      <div slot="content" class="card-padding">
         <div class="info">
         1语言：HTML5,CSS3,JS,XML,JSON,AJAX 
         </div>
        <div class="info">
         2前端框架：JQUERY MOBILE,VUE,JQUERY EASYUI,BOOTSTRAP 
        </div>
        <div class="info">
         3编辑器：Adobe Dreamweaver,Visual Studio Code,Sublime 
        </div>
        <div class="info">
         4操作系统：Windows,linux
        </div>
        <div class="info">
         5浏览器：Google Chrome， IE，Firefox 
        </div>
        <div class="info">
         6Github 网址: https://github.com/huangbin1/
        </div>
        <div class="info">
         7两年PC端和移动端前端开发经验。
        </div>
      </div>
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
        mounted() {
            console.log(this.$refs.mychart)
            var myChart = echarts.echarts.init(this.$refs.mychart);
            var option = {
                title: {
                    show: false,
                    text: '我的技能',
                    left: 'center',
                    textStyle: {
                        color: '#e683d1'
                    }
                },
                legend: {
                    show: false,
                    data: ['黄彬'],
                    // bottom: 5,
                    // left: 'right',
                    // itemGap: 20,
                    // textStyle: {
                    //     color: '#e683d1',
                    //     fontSize: 14
                    // },
                    // selectedMode: 'single'
                },
                radar: {
                    indicator: [{
                        name: 'vuejs',
                        max: 100
                    }, {
                        name: 'jquery',
                        max: 100
                    }, {
                        name: 'javascript',
                        max: 100
                    }, {
                        name: 'React',
                        max: 100
                    }, {
                        name: '微信小程序',
                        max: 100
                    }, {
                        name: '整体',
                        max: 100
                    }],
                    radius: 90,
                    shape: 'circle',
                    splitNumber: 5,
                    name: {
                        textStyle: {
                            color: "#ec6b83"
                        }
                    },
                    // splitLine: {
                    //     lineStyle: {
                    //         color: [
                    //             'rgba(238, 197, 102, 0.1)', 'rgba(238, 197, 102, 0.2)',
                    //             'rgba(238, 197, 102, 0.4)', 'rgba(238, 197, 102, 0.6)',
                    //             'rgba(238, 197, 102, 0.8)', 'rgba(238, 197, 102, 1)'
                    //         ].reverse()
                    //     }
                    // },
                    splitArea: {
                        show: false
                    },
                    axisLine: {
                        lineStyle: {
                            color: 'rgba(238, 197, 102, 0.5)'
                        }
                    }
                },
                series: [{
                    name: '黄彬',
                    type: 'radar',
                    lineStyle: {
                        normal: {
                            width: 1,
                            opacity: 0.5
                        }
                    },
                    data: [{
                        value: [80, 100, 95, 40, 50, 90],
                        name: '黄彬'
                    }],
                    symbol: 'none',
                    itemStyle: {
                        normal: {
                            color: '#F9713C'
                        }
                    },
                    areaStyle: {
                        normal: {
                            opacity: 0.1
                        }
                    }
                }]
            };
            // 使用刚指定的配置项和数据显示图表。
            myChart.setOption(option);
        },
        created: function() {
            //console.log(this.$el)
            console.log("created ")
            console.log(echarts.echarts)
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  
    .user {
        width: 100%;
        margin-bottom: 55px;
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
        font-size:0.9rem;
        color:#000000;
        border-radius:20px;
        padding: 15px;
        margin: 1rem;
        background-color: #FFCCEB;
        animation:myfirst 5s infinite;
        -moz-animation:myfirst 5s infinite; /* Firefox */
        -webkit-animation:myfirst 5s infinite; /* Safari and Chrome */
        -o-animation:myfirst 5s infinite; /* Opera */
        
    }
   @-webkit-keyframes myfirst
    {
    0%   {background:#FFFFCC;}
    25%  {background:#D1FAFA;}
    50%  {background: #E8D2E4;;}
    75%  {background: #E7A0AE;}
    100% {background:#F3CFFC;}
    }
     .photo-info p:first-child{
         font-size: 1rem;
         text-align: center;
     }
    
   
    
    .card-padding {
        padding: 15px;
    }
    
    .info {
        display: flex;
        flex-direction: row;
        font-size:0.8rem;
        color:#000000;
        white-space: nowrap;
    }
    
    .info-cat {
        flex: 1;
        font-size: 0.8rem;
        color: #000000;
    }
   
    .info-detail {
        flex: 1;
        text-align: right;
        font-size: 0.8rem;
        color: #999999;
    }
    
    .contact {
        width : 65%;
        margin: 0 auto;
    }
    #mychart {
        margin: 0 auto;
    }
    .weui-panel__hd {
    padding: 14px 15px 10px;
    color:red;
    font-size: 13px;
    position: relative;
}
</style>