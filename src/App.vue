<template>
  <div class="whole-app">
    <Header />
  </div>
</template>

<script>
import Header from './components/Header.vue'

export default {
  
  name: 'App',
  components: {
    Header
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.whole-app {
  /* width: 10rem; */
  /* height: 10rem; */
  border: 1px solid red;
  background-image: url('');
}
</style>
