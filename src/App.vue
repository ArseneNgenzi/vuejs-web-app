<template>
  <div class="whole-app">
    <Header />
    <AfterHeader />
    <Cars />
    <Footer />
    <Filter />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import AfterHeader from './components/AfterHeader.vue'
import Cars from './components/Cars.vue'
import Footer from './components/Footer.vue'
import Filter from './components/Filter.vue'

export default {
  
  name: 'App',
  components: {
    Header,
    AfterHeader,
    Cars,
    Footer,
    Filter
  }
}
</script>

<style>
#app {
  
  /* font-family: Avenir, Helvetica, Arial, sans-serif; */
  font-family: 'Work Sans', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* margin-top: 60px; */
}
.whole-app {
  /* width: 10rem; */
  /* height: 10rem; */
  /* border: 1px solid rgb(224, 224, 224); */
  /* background-image: url('../images/logo.jpg'); */
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  position: relative;
}
</style>
