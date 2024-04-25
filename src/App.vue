<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <div id="app-1">
      <p>{{msg}}</p>
      <a href="./components/work/workHome.vue" target="_blank" rel="noopener">点击我跳转到</a>
      <router-link to="/components/work/workHome.vue"><a>跳转</a></router-link>
    </div>
      <el-button>默认按钮</el-button>
  <el-button type="primary">主要按钮</el-button>
  <el-button type="success">成功按钮</el-button>
  <el-button type="info">信息按钮</el-button>
  <el-button type="warning">警告按钮</el-button>
  <el-button type="danger">危险按钮</el-button>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Vue from 'vue'

export default {

  name: 'App',
  components: {
    HelloWorld
  }
}

new Vue({
  el : '#app-1',
  data: {
    msg : 'hello zhangyan welcome'
  }
})
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
