<template>
  <div id="app">
    <div id="nav">
      <van-row type="flex" justify="space-around" >
        <van-col span="1"><router-link to="/"><van-icon name="wap-home"/> </router-link></van-col>
      </van-row>
    </div>
    <router-view/>
    <van-tabbar
      v-model="active"
      active-color="#07c160"
      inactive-color="#000"
      fixed
    >
      <van-tabbar-item icon="home-o" to="home">Home</van-tabbar-item>
      <van-tabbar-item icon="search" to="/">发现</van-tabbar-item>
      <van-tabbar-item icon="chat-o" to="message">消息</van-tabbar-item>
      <van-tabbar-item icon="setting-o" to="about">个人中心</van-tabbar-item>
    </van-tabbar>
  </div>
</template>

<script>
import Vue from 'vue'
import { Col, Row, Icon, Tabbar, TabbarItem } from 'vant'
Vue.use(Row, Col, Icon, Tabbar, TabbarItem)

export default {
  name: 'app',
  components: {
    [Row.name]: Row,
    [Col.name]: Col,
    [Icon.name]: Icon,
    [Tabbar.name]: Tabbar,
    [TabbarItem.name]: TabbarItem
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  width: 100%;
  height: 10pt;
  top: 0px;
  padding: 1rem;
  display: flex;
  position: fixed;
  z-index: 1;
  background-color: whitesmoke;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
