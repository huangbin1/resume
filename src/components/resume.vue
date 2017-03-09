<template>
  <div>
    <div id='show' v-show="choose_show">
      <show></show>
    </div>
    <div id='user' v-show="choose_user">
      <user></user>
    </div>
    <div id='project' v-show="choose_project">
      <project></project>
    </div>
    <div id='project' v-show="choose_github">
      <github></github>
    </div>
    <tabbar>
      <tabbar-item selected @on-item-click="ChooseUser(0)">
        <img slot="icon" src="../assets/show.png" >
        <span slot="label">成果展示</span>
      </tabbar-item>
      <tabbar-item selected @on-item-click="ChooseUser(1)">
        <img slot="icon" src="../assets/user.png" >
        <span slot="label">个人信息</span>
      </tabbar-item>
      <tabbar-item show-dot @on-item-click="ChooseUser(2)">
        <img slot="icon" src="../assets/project.png" >
        <span slot="label">项目</span>
      </tabbar-item>
      <tabbar-item badge="2" @on-item-click="ChooseUser(3)">
        <img slot="icon" src="../assets/github.png" >
        <span slot="label">个人项目</span>
        <div slot="default">
        <img src="../assets/github.png">
        </div>
      </tabbar-item>
    </tabbar>
  </div>
</template>

<script>
    import {
        Tabbar,
        TabbarItem,
        Group,
        Cell
    } from 'vux'

    import User from 'components/user'
    import Project from 'components/project'
    import Github from 'components/github'
    import Show from 'components/show'
    export default {
        components: {
            Show,
            User,
            Project,
            Github,
            Tabbar,
            TabbarItem,
            Group,
            Cell
        },
        data() {
            return {
                choose_user: false,
                choose_project: false,
                choose_github: false,
                choose_show: true
            }
        },
        methods: {
            ChooseUser: function(idx) {
                console.log(idx)
                this.choose_user = false
                this.choose_project = false
                this.choose_github = false
                this.choose_show = false

                if (idx == 0)
                    this.choose_show = true
                else if (idx == 1)
                    this.choose_user = true
                else if (idx == 2)
                    this.choose_project = true
                else if (idx == 3)
                    this.choose_github = true
            }
        }
    }
</script>
<style scoped>
    .weui-tabbar {
        position: fixed;
    }
</style>