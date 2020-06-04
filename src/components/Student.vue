<template>
    <div>
      <h1>学生组件</h1>
      <img src="../assets/-774826494.jpg" alt="">
      <table border="1">
        <tr>
          <td>id</td>
          <td>name</td>
          <td>age</td>
          <td>操作</td>
        </tr>
        <tr v-for="student in students">
          <td>{{student.id}}</td>
          <td>{{student.name}}</td>
          <td>{{student.age}}</td>
          <td><a href="">删除</a><a href="">修改</a></td>
        </tr>
      </table>

      <Footer></Footer>
    </div>
</template>

<script>
  import Footer from'./Footer';
    export default {
        name: "Student",
      data(){
          return{
            students:[
              {id:'1',name:'张三',age:23},
              {id:'2',name:"李四",age:58}
            ]
          }
      },
      methods:{

      },
      components:{
          Footer, //注册组件
      }
    }
</script>

<style scoped>

</style>
