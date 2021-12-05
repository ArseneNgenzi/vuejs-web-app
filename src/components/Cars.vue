<template>
  <div class="cars">
    <div class="order">
      <div class="info-prezzi">
        <div class="info-prezzi-icon">
          <i class="fa fa-external-link" aria-hidden="true"></i>
        </div>
        <div class="info-prezzi-text">
          <p>
            Info <br />
            prezzi
          </p>
        </div>
      </div>
      <div class="order-by" @click="costoMenuShow = !costoMenuShow">
        <div class="ordina-per">
          <p>Ordina per</p>
        </div>
        <div class="costo">
          <p class="costo-text">Costo</p>
          <p class="costo-unicode">&#x2335;</p>
        </div>
        <transition name="fade">
          <div class="costo-menu" v-show="costoMenuShow">
            <div id="costo">Costo</div>
            <div>Potenza</div>
            <div>Cilindrata</div>
            <div>Marca</div>
          </div>
        </transition>
      </div>
    </div>
    <!-- <img src="images/toyota.jpg" alt=""> -->
    <div class="all-cars">
     <div class="car">
      <div class="image">
       <img src="images/toyota.jpg" alt="" >
      </div>
      <div class="model-title">
       <p > 
        <span class="model">  TOYOTA PRIUS</span> 
        <span class="title">Plug-in Hybrid</span>
       </p>
      </div>
      <div class="div-with-btn">
       <div class="tipo-potenza-cilindrata">
        <div class="tipo">
         <p>Tipo: <span>Berlina</span> </p>
        </div>
        <div class="potenza">
         <p>Potenza: <span>150</span>CV | <span>110</span>kW </p>
        </div>
        <div class="cilindrata">
         <p>Cilindrata: <span>1395</span> cm <sup>3</sup> </p>
        </div>
       </div>
       <div class="tpc-btn">
        <button>PLUG-IN <br> HYBRID</button>
       </div>
      </div>
      <div class="distances">
       <div class="distance1">
        <div class="number-text-icon">
         <div class="distance1-number">5,11</div>
         <div class="distance1-text">€x100km ricarica domestica</div>
         <div class="distance-icon"><i class="fas fa-info-circle"></i></div>
        </div>
        <div class="distance-illustration">
         <div class="illu" id="illuBg"></div>
         <div class="illu"></div>
         <div class="illu"></div>
         <div class="illu"></div>
         <div class="illu"></div>
         <div class="illu"></div>
        </div>
        
       </div>
      </div>
     </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Cars',
  data() {
    return {
      costoMenuShow: false,
      cars: [
        {
          picture: 'images/vw-gray.jpg',
          model: 'VOLKSWAGEN ECO UP!',
          type: 'move 5p',
          tipo: 'Berlina',
          potenza: '150CV | 110kW',
          cilindrata: '1395 cm',
          btnText: 'GPL',
          distance1: '3,85',
          distance1Text: '€x100km per le tue abitudini',
        },
        {
          picture: 'images/ford.jpg',
          model: 'FORD FIESTA',
          type: '1.1 75 CV Gpl 5p.',
          tipo: 'Berlina',
          potenza: '150CV | 110kW',
          cilindrata: '1395 cm',
          btnText: 'GPL',
          distance1: '4,96',
          distance1Text: '€x100km',
        },
        {
          picture: 'images/hyunday.jpg',
          model: 'HYUNDAY IONIQ',
          type: 'ELECTRIC EV 38.3 kWh',
          tipo: 'Berlina',
          potenza: '150CV | 110kW',
          btnText: 'ELECTRICA',
          distance1: '3,40',
          distance1Text: '€x100km - ricarica domestica',
          distance2: '8,54',
          distance2Text: '€x100km - col. cor. continua',
        },
        {
          picture: 'images/toyota.jpg',
          model: 'TOYOTA PRIUS',
          type: 'Plug-in Hybrid',
          tipo: 'Berlina',
          potenza: '150CV | 110kW',
          cilindrata: '1395 cm',
          btnText: 'PLUG-IN HYBRID',
          distance1: '5,11',
          distance1Text: '€x100km - ricarica domestica',
          distance2: '8,54',
          distance2Text: '€x100km - col. cor. alternata',
        },
        {
          picture: 'images/toyota-blue.jpg',
          model: 'TOYOTA Prius 4a serie',
          type: '1.8 AWD Lounge',
          tipo: 'Berlina',
          potenza: '150CV | 110kW',
          cilindrata: '1395 cm',
          btnText: 'FULL HYBRID',
          distance1: '6.97',
          distance1Text: '€x100km',
        },
        {
          picture: 'images/toyota-light-blue.jpg',
          model: 'TOYOTA AYGO',
          type: '1.0 VVT-i 72 CV 5p.',
          tipo: 'Berlina',
          potenza: '150CV | 110kW',
          cilindrata: '1395 cm',
          btnText: 'BENZINA',
          distance1: '7,96',
          distance1Text: '€x100km',
        },
      ],
    }
  },
}
</script>

<style scoped>
sup {
 font-size: 0.7rem;
}
.cars {
  grid-column: 1 / -1;
}
.order {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 1.2rem;
}
.info-prezzi {
  display: flex;
  align-items: center;
}
.info-prezzi-icon {
  background-color: #eeeeee;
  padding: 0.7rem;
  border-radius: 50%;
}
.info-prezzi-icon i {
  color: rgb(77, 77, 77);
  font-size: 1.5rem;
}
.info-prezzi-text {
  text-align: left;
  margin-left: 0.5rem;
}
.info-prezzi-text p {
  color: #6e6e6ea9;
  font-size: 0.8rem;
}
.order-by {
  background-color: #eeeeee;
  display: flex;
  padding: 0.7rem;
  cursor: pointer;
  position: relative;
  /* transition: 500ms ease-in-out; */
}
.ordina-per {
  margin-right: 0.5rem;
}
.ordina-per p {
  color: rgb(77, 77, 77);
  font-weight: lighter;
}
.costo {
  display: flex;
}
.costo-text {
  font-weight: bold;
  margin-right: 2rem;
}
.costo-menu {
  border: 1px solid #6e6e6ea9;
  border-radius: 0.5rem;
  position: absolute;
  top: 3rem;
  right: 0;
  width: 100%;
  /* margin-right: 0.7rem; */
  background-color: #fff;
  /* opacity: 1;
  transition: 500ms  */
}
.costo-menu > div {
  text-align: left;
  margin: 1rem;
  font-weight: bold;
  z-index: 100;
}
#costo {
  color: rgb(250, 77, 46);
}
.fade-enter,
.fade-enter-active,
.fade-leave-active,
.fade-enter-to {
  transition: opacity 800ms;
}
.fade-enter, .fade-leave-to /* .fade-leave-active below version 2.1.8 */ {
  opacity: 0;
}
.all-cars {
 /* border: 1px solid; */
 margin: 0 1rem;
}
/* .image {
 border: 1px solid red;
} */
.car {
 border-top: 2px solid hsla(0, 0%, 43%, 0.4);
 padding-top: 1rem;
}
.image img {
 width: 100%;
 /* border: 1px solid; */
}
.model-title {
 /* display: flex; */
 padding-top: 1rem;
 padding-bottom: 1rem;
}
.model-title p {
 width: 80%;
 /* border: 1px solid; */
 text-align: left;
}
.model-title p .model {
 color: rgb(44, 44, 44);
 font-size: 1.7em;
 font-weight: bold;
 font-family: 'Work Sans', sans-serif;
 padding-right: 1rem;
}
.model-title p .title {
 font-size: 1.7rem;
 color: rgb(44, 44, 44);
 /* width: 2rem; */
}
.div-with-btn {
 display: flex;
 justify-content: space-between;
 align-items: center;
}
.div-with-btn p {
 text-align: left;
 font-size: 1.1rem;
 /* color: rgb(44, 44, 44); */
 color: rgba(49, 49, 49, 0.9)
}
.tipo-potenza-cilindrata {
 /* border: 1px solid; */
}
.tipo span, .potenza span, .cilindrata span {
 font-weight: bold;
}
.tpc-btn button {
 border: 1px solid rgb(3, 145, 3);
 color: rgb(3, 145, 3);
 font-size: 1.1rem;
 font-weight: bold;
 font-family: 'Work Sans', sans-serif;
 cursor: pointer;
 padding: 0.5rem 2rem;
}



</style>
