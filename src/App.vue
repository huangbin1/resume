<template>
  <div id="app">
    <router-view></router-view>
  </div>
</template>

<script>
    export default {
        name: 'app'
    }
</script>

<style lang="less">
    @import '~vux/src/styles/reset.less';
    /*html {
        background: #EEEEEE;
    }*/
    
    /*body {
        background: linear-gradient(to bottom right,#F4CEFD ,white);;
    }*/
    .weui-panel__hd{
        color:#FF99C2 !important;
    }
</style>