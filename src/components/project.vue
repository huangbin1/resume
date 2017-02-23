<template>
  <div class="project">
    <timeline class="timeline">
        <timeline-item>
            <h4>i80北斗RTK测量仪器二期linux应用程序开发</h4>
            <p>2015/06–2016/01</p>
        </timeline-item>
        <timeline-item>
            <h4>姿态传感器开发及应用</h4>
            <p>2015/02–2015/04</p>
        </timeline-item>
        <timeline-item>
            <h4>设备自动化检测</h4>
            <p>2014/09–2014/12</p>
        </timeline-item>
        <timeline-item>
            <h4>“挑战杯”课外学术竞赛</h4>
            <p>2012/03–2013/09</p>
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