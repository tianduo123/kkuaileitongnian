<template>
    <div class="wrap">
      <div class="search">
        <img src="../assets/search.png" style="width: 20px;height: 20px;margin: 0 10px">
        <input type="text" placeholder="搜索商品" v-model="userSearch"  @keyup.enter="search">
      </div>
      <div class="tab">
        <span @click="select1" :class="{isSelece:select=='all'}">全部</span>
        <span @click="select2" :class="{isSelece:select=='num'}">销量</span>
        <span @click="select3" :class="{isSelece:select=='price'}">价格</span>
        <span @click="select4" :class="{isSelece:select=='shangxin'}">上新</span>
      </div>
      <div class="item_wrap">
        <div class="goods_item" v-for="(goods,index) in goodsList">
          <img :src="goods.imgUrl" style="width: 80%;height: 150px">
          <div class="detail">
            <div style="text-overflow:ellipsis;white-space: nowrap;overflow: hidden">{{goods.name}}</div>
            <div style="color:#B6A786">￥{{goods.price}}</div>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
  import { Indicator } from 'mint-ui';
  export default {
        name: "store",
        data(){
          return{
            select:'all',
            goodsList:[
              {name:'JSON 实战',price:67,imgUrl:require('../assets/book.jpg')},
              {name:'JSON 实战,代发货建安费经核实对方加上就会',price:67,imgUrl:require('../assets/book.jpg')},
              {name:'JSON 实战',price:67,imgUrl:require('../assets/book.jpg')},
              {name:'JSON 实战',price:67,imgUrl:require('../assets/book.jpg')},
              {name:'JSON 实战',price:67,imgUrl:require('../assets/book.jpg')},
              {name:'JSON 实战',price:67,imgUrl:require('../assets/book.jpg')},
              {name:'JSON 实战',price:67,imgUrl:require('../assets/book.jpg')},
            ],
            userSearch:''
          }
        },
      methods:{
        select1() {
          this.select = 'all';
          Indicator.open({
            text: '加载中...',
            spinnerType: 'double-bounce'
          });
          setTimeout(()=>{
            Indicator.close()
          },1500)
        },
        select2() {
          this.select = 'num';
          Indicator.open({
            text: '加载中...',
            spinnerType: 'double-bounce'
          });
          setTimeout(()=>{
            Indicator.close()
          },1500)
        },
        select3() {
          this.select = 'price';
          Indicator.open({
            text: '加载中...',
            spinnerType: 'double-bounce'
          });
          setTimeout(()=>{
            Indicator.close()
          },1500)
        },
        select4() {
          this.select = 'shangxin',
            Indicator.open({
              text: '加载中...',
              spinnerType: 'double-bounce'
            });
          setTimeout(()=>{
            Indicator.close()
          },1500)
        },
        search(){
          alert(this.userSearch)
          this.userSearch = ''
        }
      }
    }
</script>

<style>
  .wrap{
    width: 100%;
    box-sizing: border-box;
    padding-top: 10px;
    margin-bottom: 100px;
  }
  .search{
    width: 95%;
    height: 40px;
    margin: 0 auto;
    display: flex;
    align-items: center;
    background: #fff;
    border-radius: 10px;
  }
  input{
    background:none;
    outline:none;
    border:none;
    width: 100%;
  }
  .tab{
    width: 100%;
    height: 35px;
    background: #FFF;
    margin-top: 10px;
  }
  .tab>span{
    width: 24%;
    display: inline-block;
    height: 100%;
    text-align: center;
    line-height: 35px;
    font-size: 15px;
  }
  .isSelece{
    width: 24%;
    display: inline-block;
    height: 100%;
    text-align: center;
    line-height: 35px;
    font-size: 15px;
    color: #996633;
  }
  .item_wrap{
    width: 100%;
    box-sizing: border-box;
    padding: 10px;
    font-size: 0;
  }
  .goods_item{
    display: inline-block;
    width: 47.5%;
    height: 220px;
    background: #FFF;
    margin-bottom: 10px;
    text-align: center;
    box-sizing: border-box;
    padding: 10px;
  }
  .goods_item:nth-child(odd){
    margin-right:5%;
  }
  .detail{
    font-size: 14px;
    display: flex;
    flex-direction: column;
    text-align: left;
    height: 50px;
    justify-content: space-around;
  }
</style>
