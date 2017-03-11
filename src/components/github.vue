<template>
  <div class="project">
    <timeline class="timeline">
        <timeline-item>
            <h4>云间半导体设备网页</h4>
            <div class="item_des">
            <p>2016/8–2016/08</p>
            <p><strong>项目概要:</strong>该项目是朋友公司的单片机网页</p>
            <p><strong>项目职责:</strong>优化视觉效果，兼容不同浏览器</p>
            <p><strong>项目业绩:</strong>美化了网页</p>
            </div>
        </timeline-item>
        <timeline-item>
            <h4>基于vue框架的音乐播放器(github)</h4>
            <div class="item_des">
            <p>2016/12–2017/01</p>
            <p><strong>项目概要:</strong>该项目为本人课余时间写的项目，项目代码保存在github基于vue.js框架和mintui组件，ES6写了个音乐播放器</p>
            <p><strong>项目职责:</strong>带着对前端的探索精神，独自完成整个项目</p>
            <p><strong>项目业绩:</strong>对vue，ES6 ，js，有了更深入的学习;本项目在github上有独立的开源分享</p>
            </div>
        </timeline-item>
        <timeline-item>
            <h4>基于vue框架的个人简历(github)</h4>
            <div class="item_des">
            <p>2017/02–2017/3</p>
            <p><strong>项目概要:</strong>该项目是基于vue,vux上做的一份个人简历</p>
            <p><strong>项目职责:</strong>之前用过vue，但用的是mintui组件库，这次换了vux组件库</p>
            <p><strong>项目业绩:</strong>该项目在github上已经分享</p>
            </div>
        </timeline-item>
        <timeline-item>
            <h4>基于微信小应用的二维码小助手(github)</h4>
            <div class="item_des">
            <p>2017/03–2017/03</p>
            <p><strong>项目概要:</strong>用微信小应用做了一个二维码应用，用于生成二维码和扫描二维码</p>
            <p><strong>项目职责:</strong>学习微信小应用</p>
            <p><strong>项目业绩:</strong>该项目在github上已经分享（还未完成）</p>
            </div>
        </timeline-item>
        
    </timeline>
  </div>
</template>

<script>
    import {
        Timeline,
        TimelineItem
    } from 'vux'
    export default {
        name: 'project',
        components: {
            Timeline,
            TimelineItem
        },
        data() {
            return {
                count: 3
            }
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
   
        p {
            color: #000000;
            font-size: 0.8rem;
        }
        h4 {
            color: #ffffff;
            background-color:#9A8ADC;
            text-align: center;
            font-size: 0.9rem;
            border-radius: 0.9rem;
            width: 300px;
        }
        strong{
            color: #9A8ADC;
        }
        .project{
       
        padding-bottom:3.2rem;
        }
        .item_des
        {
        border: 2px dashed #FEDEFE;
        border-radius: 10px;
        margin-top: 20px;
        background-color: #FEEFFE;
        padding:10px;
        }
 
</style>