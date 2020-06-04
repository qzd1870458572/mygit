<template>
  <div id="app">
    <!--<img src="./assets/logo.png">-->
    <!--<h1 class="aa">欢迎:{{msg}} </h1>-->
    <!--阿西吧 么么哒-->
    <!--  用来展示路由组建    -->
    <a href="#/">主页111111111</a>
    <a href="#/user">用户模块</a>
    <a href="#/student">学生模块</a>
    <router-view/>
  </div>
</template>

<script>
export default {   //es6暴露当前组件对象
  name: 'App',
  data (){
    return{
      msg: "兲"
    }
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
  margin-top: 60px;
}
  .aa{
    background-color: red;
  }
</style>
