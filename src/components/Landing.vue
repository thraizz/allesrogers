<template>
  <div class="hello">
    <img :class="getAnimation()" src="/img/index.jpg">

  </div>
</template>

<script>
import 'animate.css'
export default {
  methods: {
    getAnimation(){
      let s = "animate__infinite infinite "
      switch (Math.floor(Math.random(1)*10)) {
        case 1:
          return s+"animate__bounce"
        case 2:
          return s+"animate__rubberBand"
        case 3:
          return s+"animate__shakeX"
        case 4:
          return s+"animate__shakeY"
        case 5:
          return s+"animate__swing"
        case 6:
          return s+"animate__wobble"
        case 7:
          return s+"animate__jello"
        case 8:
          return s+"animate__heartBeat"
        case 9:
          return s+"animate__slideInRight"
        default:
          return s+"animate__bounce"
      }
    }
  }
}
</script>

<style scoped>
img { 
  width: 20vw;
  margin-left: 40vw;
  margin-top: 40vh;
  animation-duration: 1s;
  animation-iteration-count: infinite;
}
</style>