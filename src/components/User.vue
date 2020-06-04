<template>
    <div>
      <h1>用户组件</h1>
      <table border="1">
        <tr>
          <td>id</td>
          <td>name</td>
          <td>age</td>
          <td>操作</td>
        </tr>
        <tr v-for="user in users">
          <td>{{user.id}}</td>
          <td>{{user.name}}</td>
          <td>{{user.age}}</td>
          <td><a href="">删除</a><a href="">修改</a></td>
        </tr>
      </table>
      <!--使用组件-->
      <Footer></Footer>
    </div>
</template>

<script>
  import Footer from "./Footer"
    export default {
        name: "User",
      data(){
          return{
             users:[
               {id:'1',name:'张三',age:23},
               {id:'2',name:"李四",age:58}
             ]
          }
      },
      methods:{

      },
      components:{
          Footer, //注册组件
      },
     created(){ //axios

     }
    }
</script>

<style scoped>

</style>
