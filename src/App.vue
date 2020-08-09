<template>
  <div id="app">
    <landing />
  </div>
</template>

<script>
import Landing from './components/Landing.vue'

export default {
  name: 'App',
  components: {
    Landing
  }
}
</script>

<style>
body {
  background-image: url(/img/index.jpg);
  background-size: 10%;
}
</style>
