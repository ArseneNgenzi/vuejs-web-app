<template>
 
  <transition name="filtraAutoTransition">
   <div class="filtra-auto-div">
  <div class="filtra-auto-div-header">
    <h1>Filtra auto</h1>
    <button class="close-filtra-auto-div" @click="$emit('closeFiltra')">
      <!-- <i class="fa fa-times-circle" aria-hidden="true"></i> -->
      X
    </button>
  </div>

  <div class="filtra-auto-div-diagram">
   <div class="fascia-and-arrowdowm">
    <p>FASCIA DI COSTO 100KM</p>
    <h2>&#x2335;</h2>
   </div>
   <div class="fascia-diagram">
    <img src="images/fasciadiagram.jpg" alt="">
   </div>
  </div>

  <div class="alimentazione-div">
   <div class="fascia-and-arrowdowm">
    <p>ALIMENTAZIONE</p>
    <h2>&#x2335;</h2>
   </div>
   <div class="alimentazione-checkboxes">
    <label class="container">Tutte
     <input type="checkbox" checked="checked">
     <span class="checkmark"></span>
    </label>
    <label class="container">Benzina <span class="benzina-color">(123)</span>
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Gasolio <span class="gasolio-color">(71)</span>
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Mild Hybrid Benzina <span class="mild-hybrid-benzina-color">(21)</span>
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Mild Hybrid Diesel <span class="mild-hybrid-diesel-color">(5)</span>
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Full Hybrid <span class="full-hybrid-color">(15)</span>
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Plug-in Hybrid <span class="plug-in-hybrid-color">(34)</span>
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Electtrica <span class="electtrica-color">(34)</span>
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">GPL <span class="gpl-color">(6)</span>
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Metano <span class="metano-color">(6)</span>
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
   </div>
  </div>

  <div class="tipo-auto-div">
   <div class="fascia-and-arrowdowm">
    <p>TIPO AUTO</p>
    <h2>&#x2335;</h2>
   </div>
   <div class="tipo-auto-checkboxes">
    <div class="checkboxes-left">
     <label class="container">Tutte
     <input type="checkbox" checked="checked">
     <span class="checkmark"></span>
    </label>
    <label class="container">City Car
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Berlina
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Cabrio
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    </div>
    <div class="checkboxes-right">
     <label class="container">Coupé
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Station Wagon
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Monovolume
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Suv/Fuoristr.
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    </div>
   </div>
   <!-- <div class="tipo-auto-checkboxes">

    <label class="container">Tutte
     <input type="checkbox" checked="checked">
     <span class="checkmark"></span>
    </label>
    <label class="container">Benzina <span class="benzina-color">(123)</span>
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Gasolio <span class="gasolio-color">(71)</span>
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Mild Hybrid Benzina <span class="mild-hybrid-benzina-color">(21)</span>
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Mild Hybrid Diesel <span class="mild-hybrid-diesel-color">(5)</span>
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Full Hybrid <span class="full-hybrid-color">(15)</span>
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Plug-in Hybrid <span class="plug-in-hybrid-color">(34)</span>
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Electtrica <span class="electtrica-color">(34)</span>
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">GPL <span class="gpl-color">(6)</span>
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Metano <span class="metano-color">(6)</span>
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
   </div> -->
  </div>

  <div class="marca-div">
   <div class="fascia-and-arrowdowm">
    <p>MARCA</p>
    <h2>&#x2335;</h2>
   </div>
   <div class="tipo-auto-checkboxes">
    <div class="checkboxes-left">
     <label class="container">Tutte
     <input type="checkbox" checked="checked">
     <span class="checkmark"></span>
    </label>
    <label class="container">Alpha Romeo
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Alpine
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Aston Martin
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Audi
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">BMW
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Citroen
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Cupra
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Dacia
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Ds
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Dr
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Fiat
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Ford
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Honda
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Hyundai
     <input type="checkbox" >
     <span class="checkmark"></span>
    </label>
    <label class="container">Jaguar
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Jeep
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Kia
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Lancia
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Land Rover
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Lexus
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    </div>
    <div class="checkboxes-right">
     <label class="container">Mahindra
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Mazda
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Mercedes
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Mg
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Mini
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Mitsubishi
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Nissan
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Opel
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Peugeot
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Porsche
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Renault
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Seat
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Skoda
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Ssangyong
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Subaru
     <input type="checkbox" >
     <span class="checkmark"></span>
    </label>
    <label class="container">Suzuki
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Toyota
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Tesla
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Volkswagen
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Volvo
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    <label class="container">Xev
     <input type="checkbox">
     <span class="checkmark"></span>
    </label>
    </div>
   </div>
  </div>


  <!-- 88 AUTO -->
  <div class="_88-auto">
    <h1>88 auto</h1>
    <p>Vai alla lista</p>
  </div>
</div>
  </transition>
  
 
</template>

<script>
 export default {
  name: 'FiltraAuto',
  data(){
   return {

   }
  },
  emits: ['closeFiltra']
 }
</script>

<style scoped>
.filtra-auto-div {
   position: absolute;
   background-color: #fff;
   /* grid-column: 1 / -1; */
   left: 0;
   top: 0;
   width: 100%;
   /* bottom: 0; */
   /* height: 80rem; */
   z-index: 1;
   /* overflow-y: scroll;
   scroll-behavior: smooth; */
   /* border: 1px solid; */
   padding-bottom: 6rem;
 }
 .filtra-auto-div-header {
   border-bottom: 1px solid #c1c1c1;
   display: flex;
   justify-content: space-between;
   margin: 0 1rem;
   padding: 2rem 0;
 }
 .close-filtra-auto-div {
   font-size: 2.5em;
   padding: 0 0.6rem;
   border-radius: 50%;
   border: 0;
   outline: none;
   color: #fff;
   background-color: rgb(250, 77, 46);
   cursor: pointer;
   position: fixed;
   right: 1rem;
   z-index: 2;
 }
 .filtra-auto-div-diagram {
  margin: 1rem;
  border-bottom: 1px solid #c1c1c1;
 }
 .fascia-and-arrowdowm {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 0.5rem;
  padding-bottom: 1rem;
 }
 .fascia-and-arrowdowm p {
  color: rgb(250, 77, 46);
  font-weight: bold;
  font-size: 1.3rem;
  /* letter-spacing: 0.1em; */
 }
 .fascia-and-arrowdowm h2 {
  color: #aaaaaa;
  font-size: 1.9rem;
 }
 .fascia-diagram img {
  width: 100%;
  /* height: 100%; */
  /* height: 5rem; */
 }
 .alimentazione-div {
  margin: 1rem;
  border-bottom: 1px solid #c1c1c1;
  /* margin-bottom: 2rem; */
 }
 .tipo-auto-div {
  margin: 1rem;
  border-bottom: 1px solid #c1c1c1;
 }
 .marca-div {
  margin: 1rem;
  border-bottom: 1px solid #c1c1c1;
 }

 /* START OF CHECKBOXES */

 /* The container */
.container {
  display: flex;
  /* justify-content: space-around; */
  position: relative;
  /* padding-left: 35px; */
  margin-bottom: 1rem;
  cursor: pointer;
  font-size: 1.2rem;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
  /* border: 1px solid; */
  width: auto;
  padding-left: 2rem;
  color: #000000;
  /* font-weight: bold; */
}

/* Hide the browser's default checkbox */
.container input {
  position: absolute;
  opacity: 0;
  cursor: pointer;
  height: 0;
  width: 0;
  /* display: none; */
}

/* Create a custom checkbox */
.checkmark {
  position: absolute;
  top: 0;
  left: 0;
  height: 25px;
  width: 25px;
  /* background-color:rgb(250, 77, 46); */
  border-radius: 5px;
  border: 1px solid #c1c1c1;
  /* margin-right: 1rem; */
}

/* On mouse-over, add a grey background color */
.container:hover input ~ .checkmark {
  /* background-color: #ccc; */
}

/* When the checkbox is checked, add a orange background */
.container input:checked ~ .checkmark {
  background-color: rgb(250, 77, 46);
  border: 1px solid #c1c1c1;
  border-radius: 50%;
  padding: 0.5rem;
  /* color: rgb(250, 77, 46); */
}

/* Create the checkmark/indicator (hidden when not checked) */
.checkmark:after {
  content: "";
  position: absolute;
  display: none;
  /* color: rgb(250, 77, 46); */
}

/* Show the checkmark when checked */
.container input:checked ~ .checkmark:after {
  display: block;
  /* color: rgb(250, 77, 46); */
}

/* Style the checkmark/indicator */
.container .checkmark:after {
  left: 8px;
  top: 4px;
  width: 5px;
  height: 10px;
  border: solid white;
  border-width: 0 3px 3px 0;
  -webkit-transform: rotate(45deg);
  -ms-transform: rotate(45deg);
  transform: rotate(45deg);
  /* color: rgb(250, 77, 46); */
}

 /* END OF CHECKBOXES */


.benzina-color {
 margin-left: 0.3rem;
 color: #e20000;
}
.gasolio-color {
 margin-left: 0.3rem;
 color: #707070;
}
.mild-hybrid-benzina-color, .mild-hybrid-diesel-color {
 margin-left: 0.3rem;
 color: #009933;
}
.full-hybrid-color {
 margin-left: 0.3rem;
 color: #88b31a;
}
.plug-in-hybrid-color, .electtrica-color, .gpl-color, .metano-color {
 margin-left: 0.3rem;
 color: #000000;
}

/* .tipo-auto-checkboxes > .container {
 width: 50%;
 float: left;
 height: fit-content;
} */
.tipo-auto-checkboxes {
 display: flex;
 justify-content: space-between;
 padding-bottom: 1rem;
}
.checkboxes-right {
 margin-right: 1rem;
}




 ._88-auto {
   background-color: rgb(250, 77, 46);
   position: fixed;
   bottom: 0;
   left: 0;
   width: 100%;
   padding: 0.13rem;
 }
 ._88-auto h1 {
   color: #fff;
 }
 ._88-auto p {
   color: #fff;
   font-size: 1.5em;
 }



 .filtraAutoTransition-enter-from {
  opacity: 0;
 }
 .filtraAutoTransition-enter-to {
  opacity: 1;
 }
 .filtraAutoTransition-enter-active {
  transition: opacity 500ms ease-in-out;
 }
 .filtraAutoTransition-leave-from {
  opacity: 1;
 }
 .filtraAutoTransition-leave-to {
  opacity: 0;
 }
 .filtraAutoTransition-leave-active {
  transition: opacity 500ms ease-in-out;
 }
 

</style>