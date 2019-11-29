<template>
  <div>
    <mt-swipe :auto="4000" style="height:200px;width:100%;">
      <mt-swipe-item style="background: yellowgreen">
        <img src="../assets/01.jpg" style="width: 100%;height: 100%">
      </mt-swipe-item>
      <mt-swipe-item style="background: yellowgreen">
        <img src="../assets/02.png" style="width: 100%;height: 100%">
      </mt-swipe-item>
      <mt-swipe-item style="background: yellowgreen">
        <img src="../assets/01.jpg" style="width: 100%;height: 100%">
      </mt-swipe-item>
    </mt-swipe>
  </div>
</template>

<script>
    export default {
        name: "swiper",
        methods:{
        }
    }
</script>

<style>

</style>
