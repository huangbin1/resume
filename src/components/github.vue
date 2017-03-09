<template>
  <div class="project">
    <timeline class="timeline">
        <timeline-item>
            <h4>云间半导体设备网页</h4>
            <p>2016/8–2016/08</p>
            <p><strong>项目概要:</strong>该项目是见最近微信小程序比较火，课余时间用微信小应用做了一个二维码应用</p>
            <p><strong>项目职责:</strong>因为对新鲜的微信小程序特别好奇，有UI设计，js，html的基础，所以独自做了该项目</p>
            <p><strong>项目业绩:</strong>功能是实现二维码扫描和二维码生成，该项目在github上已经分享</p>
           
        </timeline-item>
        <timeline-item>
            <h4>基于vue框架的音乐播放器(github)</h4>
            <p>2016/12–2017/01</p>
            <p><strong>项目概要:</strong>该项目为本人课余时间写的项目，项目代码保存在github
          基于vue.js框架和mintui组件，ES6写了个音乐播放器</p>
            <p><strong>项目职责:</strong>带着对前端的探索精神，独自完成整个项目</p>
            <p><strong>项目业绩:</strong>对vue，ES6 ，js，有了更深入的学习;本项目在github上有独立的开源分享</p>
        </timeline-item>
        <timeline-item>
            <h4>基于vue框架的个人简历(github)</h4>
            <p>2017/02–2017/3</p>
            <p><strong>项目概要:</strong>该项目是基于vue,vux上做的一份个人简历</p>
            <p><strong>项目职责:</strong>之前用过vue，但用的是mintui组件库，这次换了vux组件库</p>
            <p><strong>项目业绩:</strong>该项目在github上已经分享</p>
        </timeline-item>
        <timeline-item>
            <h4>基于微信小应用的二维码小助手(github)</h4>
            <p>2017/03–2017/03</p>
            <p><strong>项目概要:</strong>该项目是见最近微信小程序比较火，课余时间用微信小应用做了一个二维码应用</p>
            <p><strong>项目职责:</strong>因为对新鲜的微信小程序特别好奇，有UI设计，js，html的基础，所以独自做了该项目</p>
            <p><strong>项目业绩:</strong>功能是实现二维码扫描和二维码生成，该项目在github上已经分享</p>
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
            color: #F9B0B0;
            font-size: 0.8rem;
        }
        h4 {
            color: #F9B0B0;
            font-weight: normal;
        }
        strong{
            color: #F9B0B0;
            font-size: 0.6rem;
        }
 
</style>