<template>
  <div id="app">
    <img src="./assets/logo.png">
    <h>黄彬的简历</h>
    <md-button>Default</md-button>
    <md-button class="md-primary">Primary</md-button>
    <md-button class="md-accent">Accent</md-button>
    <md-button class="md-warn">Warn</md-button>
    <md-button class="md-primary" disabled>Disabled</md-button>
    <md-button class="md-dense">Dense</md-button>
    <router-view>ddddd</router-view>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
