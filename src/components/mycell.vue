<template>
  <div class="info">
    <div class="info-cat">出生年月</div>
    <div class="info-detail">1992年02月14日</div>
  </div>
</template>

<script>
    export default {
        name: 'mycell'
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
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