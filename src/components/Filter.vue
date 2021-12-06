<template>

 <div class="filter">
   <i class="fa fa-sliders" aria-hidden="true"></i>
  <button class="filter-btn">
   Filtra auto
  </button>
 </div>
</template>

<script>
 export default {
  name: 'Filter',
 }
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Work+Sans:wght@800&display=swap');

 .filter {
  /* grid-column: 1 / -1; */
  position: fixed;
  bottom: 0;
  background-color: rgb(250, 77, 46);
  /* opacity: 1; */
  width: 100%;
  display: flex;
  align-items: center;
  
 }
 .filter-btn {
  background-color: rgb(250, 77, 46);
  border: 0;
  outline: none;
  width: 100%;
  color: #fff;
  font-family: 'Work Sans', sans-serif;
  font-size: 2rem;
  font-weight: bold;
  padding: 1rem 0;
  cursor: pointer;
  /* flex: 1; */
 }
 .filter .fa {
  /* flex: 0; */
  color: #fff;
  font-size: 2rem;
  margin-left: 1rem;
 }
 
</style>