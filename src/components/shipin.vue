<template>
  <div>
  <div class="header">视频</div>
  <div class="video_wrap">
      <div class="video_item" v-for="(item,index) in videoList" :key="index">
        <img :src="item.imgUrl" style="width: 60px;height: 60px;">
        <div style="">{{item.title}}</div>
        <img src="../assets/rightjt.png" style="width: 30px;height: 30px;">
      </div >
    </div>
  </div>
</template>

<script>
    export default {
      data(){
        return{
          videoList:[
            {imgUrl:require('../assets/02.png'),title:'课程理念及说课讲解'},
            {imgUrl:require('../assets/02.png'),title:'中班语言能力第一册'},
            {imgUrl:require('../assets/02.png'),title:'小班语言能力第一册'},
            {imgUrl:require('../assets/02.png'),title:'小学数学逻辑思维训练第一册'},
            {imgUrl:require('../assets/02.png'),title:'中班数学逻辑思维训练第一册'},
          ]
        }
      }
    }
</script>

<style>
  .header{
    width: 100%;
    height: 50px;
    text-align: center;
    line-height: 50px;
    background: linear-gradient(#667eea,#764ba2);
    color: #FFFFFF;
    margin-bottom: 10px;
  }
  .video_wrap{
    box-sizing: border-box;
    margin: 10px;
  }
  .video_item{
    width: 100%;
    height: 80px;
    background: #ffffff;
    margin-bottom: 10px;
    display: flex;
    align-items: center;
    box-sizing: border-box;
    padding: 10px;
    justify-content: space-between;
  }

</style>
