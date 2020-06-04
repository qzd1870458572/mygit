<template>
   <div>
     <h1>主页组件Home</h1>
     <div class="label">数据内容</div>
     <!--使用组件-->
     <Footer>{{}}</Footer>
   </div>
</template>

<script>
  import Footer from  './Footer'
    export default {
        name: "Home",
      data(){
          return{

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
.label{
  width: 100%;
  height: 300px;
  background-color: greenyellow;
}
</style>
