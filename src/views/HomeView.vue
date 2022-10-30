<script setup>
import TheWelcome from '../components/TheWelcome.vue'
</script>

<template>
  <div id="HomepageContainer">
    <div class="headerimg">
      <img src="/headerimg.jpg">
    </div>
    <div class="report">
      <div class="greenBox">
        阴性
      </div>
      <div class="textBox">
        <h1>72 小时内</h1>
        <h2>{{reportTime}}</h2>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name:"Homepage",
  data(){
    return{
      Opentime:"",
      reportTime:"报告时间：",
    }
  }
}
</script>
<style lang="scss" scoped>
#HomepageContainer{
  display: flex;
  flex-direction: column;
  .headerimg{
    width: 100%;
    img{
      width: 100%;
      height: auto;
    }
  }
  .report{
    display: flex;
    .greenBox{
      margin-left: 8px;
      height: 70px;
      width: 70px;
      font-size: 28px;
      background-color: #6DA973;
      color: white;
      display: flex;
      font-family: 'Sim Hei';
      font-weight: 600;
      justify-content: center;
      
      align-items: center;
      text-align: center;
    }
    .textBox{
      display: flex;
      flex-direction: column;
      justify-content: space-evenly;
      margin-left: 10px;
      h1{
        font-size: 19px;
        font-weight: 500;
        color: black;
      }
      h2{
        
      font-family: '微软雅黑';
        font-size: 20px;
        font-weight: 500;
        color: #007BFF;
      }
    }
  }
}
</style>