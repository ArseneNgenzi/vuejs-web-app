<template>
 <div class="header">
  <div class="logo">
   <div class="orange-line-logo"></div>
   <div class="logo-words">
    <div class="logo-Q">Q</div>
    <div class="logo-premium-dots">
     <h1 class="premium-word">PREMIUM</h1>
     <div class="dots">
      <div class="dot"></div>
      <div class="dot"></div>
      <div class="dot"></div>
      <div class="dot"></div>
     </div>
    </div>
   </div>
  </div>
  <div class="burger-menu">bar</div>
 </div>
</template>

<script>
 export default {
  name: 'Header',
 }
</script>

<style scoped>
.header {
 
 display: flex;
 justify-content: space-between;
 align-items: center;
}
.logo {
 background-color: yellow;
 width: 70%;
}
.orange-line-logo {
 width: 40%;
 height: 0.3rem;
 background-color: rgb(255, 115, 0);
}
.burger-menu {
 /* width: 50%; */
 background-color: red;

}
.logo-words {
 display: flex;
 align-items: center;
}
.logo-Q {
 font-size: 3em;
 font-weight: bolder;
 color: rgb(255, 115, 0);
}
.premium-word {
 font-weight: bolder;
 font-size: 1.5em;
 letter-spacing: 0.1em;
}
.dots {
 display: flex;
}
.dot {
 width: 0.5rem;
 height: 0.5rem;
 background-color: rgb(255, 115, 0);
 margin-right: 0.1rem;
 border-radius: 50%;
}
</style>