<template>
  <div>
    <div class="navigate">
      <div class="navigate_item" v-for="(navigate,index) in navigateList">
        <img :src="navigate.imgUrl" class="icon">
        <span>{{navigate.title}}</span>
      </div>
    </div>
    <div class="line"></div>
    <div class="kc_wrap">
      <div class="kc_top">
        <div>
          <img src="../assets/video.svg" style="width: 30px;height: 30px">
          <span style="margin-left: 10px;font-weight: bold;font-size: 15px;">独家特色课</span>
        </div>
        <span style="color: #666;font-size: 14px">更多>></span>
      </div>
      <div class="kc_item">
        <div class="item_tl">
          <div class="teacher">
            <img src="../assets/teacher.svg" style="width:20px;height: 20px;">
            <span style="margin-left: 10px">主讲人 快乐童年</span>
          </div>
          <div class="content">
            哈是否鉴定符几啊的积分和可敬的房间看大富科技哈加速度快回复案件是否阿积分兑换家电话费按计划
          </div>
        </div>
        <div class="item_tr" >
          <img src="../assets/02.png" style="width: 100%;height: 100%;z-index: -1" alt="">
          <img src="../assets/play.svg" style="width: 50px;height: 50px;position: absolute" @click="play"  name="01">
        </div>
        <div class="item_bl">
          <img src="../assets/02.png" style="width: 100%;height: 100%;z-index: -1" alt="">
          <img src="../assets/play.svg" style="width: 50px;height: 50px;position: absolute" @click="play"  name="02">
        </div>
        <div class="item_br">
          <div class="teacher">
            <img src="../assets/teacher.svg" style="width:20px;height: 20px;">
            <span style="margin-left: 10px">主讲人 快乐童年</span>
          </div>
          <div class="content">
            哈是否鉴定符几啊的积分和可敬的房间看大富科技哈加速度快回复案件是否阿积分兑换家电话费按计划
          </div>
        </div>
      </div>
      <img src="../assets/04.png" style="margin-top: 10px;width: 100%;margin-bottom: 100px">
    </div>
  </div>
</template>

<script>

    export default {
      name: "navigate",
      data(){
        return{
          navigateList:[
            {title:'备课上课',imgUrl:require('../assets/shangke.png')},
            {title:'理念及课程',imgUrl:require('../assets/linian.png')},
            {title:'名园建设',imgUrl:require('../assets/build.png')},
            {title:'加入联盟',imgUrl:require('../assets/join.png')}
          ], //导航0
          kcList:[
            {title:'这是独家特色课标题1'},
            {title:'这是独家特色课标题2'},
          ]
        }
      },
      methods:{
        play(){

        }
      },
      props:{

      },
    }
</script>

<style>
  .navigate{
    width: 100%;
    height: 100px;
    display: flex;;
    align-items: center;
    justify-content: space-around;
  }
  .icon{
    width:50px;
    height: 50px;
  }
  .navigate_item{
    width: 25%;
    height: 80px;
    display: flex;
    align-items: center;
    flex-direction: column;;
    justify-content: space-around;
    font-size: 14px;
  }
  .line{
    width: 100%;
    height: 10px;
    background: #ccc;
  }
  .kc_wrap{
    width: 100%;
    box-sizing: border-box;
    padding-left: 10px;
    padding-right: 10px;
  }
  .kc_top{
    width: 100%;
    height: 30px;
    display: flex;
    align-items: center;
    justify-content: space-between;

  }
  .kc_top>div{
    display: flex;
    align-items: center;
    width: 50%;
  }
  .kc_item{
    width: 100%;
    height: 400px;
    display: flex;
    color: #FFFFFF;
    font-size: 12px;
    flex-wrap: wrap;
  }
  .item_tl{
    width: 50%;
    height: 50%;
    box-sizing: border-box;
    padding: 10px;
    background:#E56D2E
  }
 .item_tr{
   width: 50%;
   height: 50%;
   display: flex;
   align-items: center;
   justify-content: space-around;
   background: rgba(0,0,0,.5);
  }
 .item_bl{
   width: 50%;
   height: 50%;
   display: flex;
   align-items: center;
   justify-content: space-around;
   background: rgba(0,0,0,.5);
 }
 .item_br{
   width: 50%;
   height: 50%;
   box-sizing: border-box;
   padding: 10px;
   background:#E56D2E
 }
 .teacher{
    display: flex;
    align-items: center;
    height: 30px;
    border-bottom: 1px solid #FFFFFF;
    margin-bottom: 10px;
  }
</style>
