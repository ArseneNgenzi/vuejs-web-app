<template>
 <div class="header">
  <div class="logo">
   <img src="images/logo.jpg" alt="">
  </div>
  <div class="burger-menu">
   <img src="images/burger.jpg" alt="">
  </div>
 </div>
</template>

<script>
 export default {
  name: 'Header',
 }
</script>

<style scoped>
.header {
 grid-column: 1 / -1;
 display: flex;
 justify-content: space-between;
 align-items: center;
 box-shadow: 5px 5px 10px 2px rgba(145, 145, 145, 0.5);
 position: sticky;
 top: 0;
 background-color: #fff;
 /* width: 100%; */
}
.logo {
  width: fit-content;
  height: fit-content;
}
.burger-menu {
  margin: 0 1rem;
}
</style>