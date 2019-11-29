<template>
    <div>
      <!--用户信息-->
      <div class="myTop">
        <div class="myInfo1">
          <img src="../assets/03.jpg" style="width: 60px;height: 60px;border-radius: 50%;margin-left: 10px">
          <div>
            <span>用户名</span>
            <span>会员身份:喵喵园长</span>
          </div>
          <img src="../assets/rightjt2.png" style="width: 20px;height: 20px">
        </div>
        <div class="myInfo2">
          <div class="price_item">
            <div>1234.55</div>
            <div style="color: #000000;font-size: 15px;margin-top: 10px">账户余额</div>
          </div>|
          <div class="price_item">
            <div>1234</div>
            <div style="color: #000000;font-size: 15px;margin-top: 10px">我的充值</div>
          </div>|
          <div class="price_item">
            <div>1234</div>
            <div style="color: #000000;font-size: 15px;margin-top: 10px">我的消费</div>
          </div>
        </div>
      </div>
      <!--底部菜单-->
      <div class="myMenu">
        <div class="menu_item">
          <img src="../assets/myOrder.svg" style="width: 30px;height: 30px;vertical-align: middle;margin-left: 10px">
          <span style="margin-left: 10px">我的订单</span>
          <span style="float: right;margin-right: 15px"> > </span>
        </div>
        <div class="menu_item">
          <img src="../assets/myAccount.svg" style="width: 30px;height: 30px;vertical-align: middle;margin-left: 10px">
          <span style="margin-left: 10px">我的账户</span>
          <span style="float: right;margin-right: 15px"> > </span>
        </div>
        <div class="menu_item">
          <img src="../assets/myCart.svg" style="width: 30px;height: 30px;vertical-align: middle;margin-left: 10px">
          <span style="margin-left: 10px">我的购物车</span>
          <span style="float: right;margin-right: 15px"> > </span>
        </div>
        <div class="menu_item">
          <img src="../assets/myLike.svg" style="width: 30px;height: 30px;vertical-align: middle;margin-left: 10px">
          <span style="margin-left: 10px">我的收藏</span>
          <span style="float: right;margin-right: 15px"> > </span>
        </div>
        <div class="menu_item">
          <img src="../assets/myIdea.svg" style="width: 30px;height: 30px;vertical-align: middle;margin-left: 10px">
          <span style="margin-left: 10px">意见反馈</span>
          <span style="float: right;margin-right: 15px"> > </span>
        </div>
        <div class="menu_item">
          <img src="../assets/mySet2.svg" style="width: 30px;height: 30px;vertical-align: middle;margin-left: 10px">
          <span style="margin-left: 10px">我的设置</span>
          <span style="float: right;margin-right: 15px"> > </span>
        </div>
      </div>
    </div>
</template>

<script>
    export default {
        name: "myself"
    }
</script>

<style>
  .myTop{
    width: 100%;
    height: 200px;
    background: linear-gradient(#f83600,#fee140);
    box-sizing: border-box;
    padding: 10px;
  }
  .myInfo1,.myInfo2{
    width: 100%;
    height: 90px;
    display: flex;
    align-items: center;
  }
  .myInfo1>div{
    display: flex;
    flex-direction: column;
    margin-left: 20px;
    width: 100%;
    color: #FFFFFF;
    font-size: 15px;
  }
  .myInfo2{
    justify-content: space-around;
  }
  .price_item{
    display: flex;
    align-items: center;
    flex-direction: column;
    color: #ffffff;
  }
  .myMenu{
    width: 100%;
    background: #FFFFFF;
  }
  .menu_item{
    width: 100%;
    border-bottom: 1px solid #666;
    height: 50px;
    line-height: 50px;
    font-size: 15px;
  }
</style>
