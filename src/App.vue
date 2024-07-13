<template>
  <div>
    <MyHeader/>
  </div>
  <div>
    <Banner/>
  </div>
  <div>
    <News/>
  </div>
</template>

<script>
import MyHeader from './components/Header.vue'
import Banner from './components/Banner.vue'
import News from './components/News.vue'

export default {  
  name: 'App',
  components: {
    MyHeader,
    Banner,
    News
  }
}
</script>

<style>
body {
  background-color: #f25241;
}
</style>
