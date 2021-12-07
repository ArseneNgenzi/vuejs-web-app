<template>
  <div class="afterheader">
   <div class="afterheader-orange-text">
    <!-- <img src="images/ex100km.jpg" alt=""> -->
    <div class="ex100km">
     <div class="eurologo">
      <p>&euro;</p>
     </div>
     <div class="x">
      <p>X</p>
     </div>
     <div class="100km">
      <div class="_100">
       <p>100</p>
      </div>
      <div class="km">
       <p>KM</p>
      </div>
     </div>
    </div>
    <p class="piuinfo">I costi chilometrici relativi alle auto <br> provate dal 2016 ad oggi. <span> <a href="">Più info</a> </span> </p>
   </div>
   <div class="afterheader-h4">
    <p>COSTI CALCOLATI <br> SU QUESTE PERCENTUALI DI UTILIZZO</p>
   </div>
   <div class="afterheader-numbers-colors">
    <div class="numbers-33">
     <div class="_33">
     <div class="yellow nbr33">33</div>
     <div id="citta" class="word33">CITTÀ</div>
    </div>
    <div class="_33">
     <div class="blue nbr33">33</div>
     <div id="statale" class="word33">STATALE</div>
    </div>
    <div class="_33">
     <div class="green nbr33">33</div>
     <div id="autostrada" class="word33">AUTOSTRADA</div>
    </div>
    </div>
    <div class="colors">
     <div class="yellow-line"></div>
     <div class="blue-line"></div>
     <div class="green-line"></div>
    </div>
   </div>
   <button class="afterheadbtn"> <img src="images/cambia.jpg" alt=""></button>
  </div>
</template>

<script>
export default {
  name: 'AfterHeader',
  data(){
   return {
    // orderByShow: false,
   }
  }
}
</script>


<style scoped>

  @import url('https://fonts.googleapis.com/css2?family=Work+Sans:wght@500&display=swap');

 .afterheader {
  grid-column: 1 / -1;
  background-color: #eeeeee;
  margin-top: 0.2rem;
 }
 .afterheader-orange-text {
  background-color: #fff;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 1em;
 }
 .piuinfo {
  padding: 1em 0.4em 1em 1em;
  font-size: 0.8em;
  color: #6e6e6e;
 }
 .piuinfo span a {
  color: rgb(250, 77, 46);
  font-weight: bold;
 }
 .ex100km {
  display: flex;
  align-items: center;
  justify-content: space-between;
 }
 .eurologo p {
  color: rgb(250, 77, 46);
  font-size: 3rem;
  /* font-family: Helvetica ; */
  font-family: 'Montserrat', sans-serif;
  /* font-weight: 500; */
 }
 .x {
  color: rgb(250, 77, 46);
  font-size: 2.5rem;
  font-family: 'Montserrat', sans-serif;
 }
 ._100 p {
  color: rgb(250, 77, 46);
  font-size: 1rem;
  font-family: 'Montserrat', sans-serif;
  font-weight: bold;
 }
 .km p {
  color: rgb(250, 77, 46);
  font-size: 1rem;
  font-family: 'Montserrat', sans-serif;
  font-weight: bold;
  /* margin: 0; */
 }
 .afterheader-h4 {
  padding: 1em 0;
  
 }
 .afterheader-h4 p {
   font-weight: bold;
   font-family: 'Work Sans', sans-serif;
   color: #333333;
 }
 .numbers-33 {
  display: flex;
  padding: 0 1em;
 }
 ._33 {
  background-color: #fff;
  border-radius: 0.5em;
  width: 32%;
  margin: 0 auto;
  padding: 0.3em 0;
  display: flex;
  flex-direction: column;
  justify-content: center;
 }
 .nbr33 {
  font-size: 2em;
  font-weight: bold;
  /* font-family: Arial, Helvetica, sans-serif; */
  font-family: 'Work Sans', sans-serif;
 }
 .yellow {
  /* color: rgb(245, 190, 40); */
  color: #ffc31f;
  
 }
 .blue {
  color: #3e97ff;
  /* color: rgb(0, 118, 165); */
 }
 .green {
  color: #26be0a;

 }
 .word33 {
  color: #6e6e6e;
  font-weight: bold;
 }

 .colors {
  margin: 1em 1em 0 1em;
  display: flex;
  justify-content: space-between;
 }
 .colors > div {
  height: 0.8em;
  width: 33.5%;
  
 }
 .yellow-line {
  background-color: #ffc31f;
 }
 .blue-line {
  background-color: #3e97ff;
 }
 .green-line {
  background-color: #26be0a;
 }
 .afterheadbtn {
  color: rgb(250, 77, 46);
  font-size: 1em;
  font-weight: bold;
  font-family: inherit;
  background-color: #fff;
  border: none;
  outline: none;
  padding: 0.5em;
  width: 90%;
  margin: 1rem auto;
  border-radius: 0.5rem;
  cursor: pointer;
 }
</style>
