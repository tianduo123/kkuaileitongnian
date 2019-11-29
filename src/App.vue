<template>
  <div>
    <mt-tab-container v-model="selected">
      <mt-tab-container-item id="one">
        <swiper></swiper>
        <navigate></navigate>
      </mt-tab-container-item>
      <mt-tab-container-item id="two">
        <store></store>
      </mt-tab-container-item>
      <mt-tab-container-item id="three">
        <Video></Video>
      </mt-tab-container-item>
      <mt-tab-container-item id="four">
        <myself></myself>
      </mt-tab-container-item>
    </mt-tab-container>
    <div class="bottom-bar">
      <mt-tabbar v-model="selected" :fixed='true' style="border-top: 1px solid #cccccc;background: #ffffff">
        <mt-tab-item id="one">
          <img slot="icon" src="./assets/home.png">
          首页
        </mt-tab-item>
        <mt-tab-item id="two">
          <img slot="icon" src="./assets/store.png">
          商城
        </mt-tab-item>
        <mt-tab-item id="three">
          <img slot="icon" src="./assets/video.png">
          视频
        </mt-tab-item>
        <mt-tab-item id="four">
          <img slot="icon" src="./assets/me.png">
          我的
        </mt-tab-item>
      </mt-tabbar>
    </div>
  </div>
</template>

<script>
  import swiper from './components/swiper'
  import navigate from './components/navigate'
  import store from './components/store'
  import Video from './components/shipin'
  import myself from './components/myself'

  export default {
    name: 'App',
    data(){
      return{
        selected:'one'
      }
    },
    components:{
      swiper,
      navigate,
      store,
      Video,
      myself
    }
  }
</script>

<style>
  body{margin: 0;
    background: #eeeeee;
  }
</style>
