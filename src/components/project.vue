<template>
  <div class="project">
    <timeline class="timeline">
        <timeline-item>
            <h4>mc100压石项目网页(mobile)</h4>
            <p>2015/03–2015/07</p>
        </timeline-item>
        <timeline-item>
            <h4>驾考定位视频监控系统网页(pc)</h4>
            <p>2015/03–2015/07</p>
        </timeline-item>
        <timeline-item>
            <h4>N72 CORS北斗参考站接收机网页(pc,mobile)</h4>
            <p>2015/06–2015/10</p>
        </timeline-item>
        <timeline-item>
            <h4>i80北斗RTK测量仪器的自动化检测系统网页(pc,mobile)</h4>
            <p>2015/10--2017/03</p>
        </timeline-item>
        <timeline-item>
            <h4>中兵集团，千寻位置，接收机定位系统(pc)</h4>
            <p>2016/01–2017/02</p>
        </timeline-item>
        <timeline-item>
            <h4>接收机PC网页UI改版(pc)</h4>
            <p>2016/09–2016/12</p>
        </timeline-item>
        <timeline-item>
            <h4>高精度板卡网页(pc)</h4>
            <p>2016/04–2016/08 </p>
        </timeline-item>
        <timeline-item>
            <h4>无人船测深仪项目(pc,mobile)</h4>
            <p>2017/01–2017/02</p>
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
    .timeline {
        p {
            color: #888;
            font-size: 0.8rem;
        }
        h4 {
            color: rgb(4, 190, 2);
            font-weight: normal;
        }
    }
</style>