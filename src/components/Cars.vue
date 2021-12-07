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
    <div class="all-cars" >

              <div class="car" v-for="car in cars" :key="car.id">
      <div class="image">
       <img :src="car.picture" alt="" >
      </div>
      <div class="model-title">
       <p > 
        <span class="model" v-html="car.model">  </span> 
        <span class="title" v-html="car.type">  </span>
       </p>
      </div>
      <div class="div-with-btn">
       <div class="tipo-potenza-cilindrata">
        <div class="tipo">
         <p>Tipo: <span> {{car.tipo}} </span> </p>
        </div>
        <div class="potenza">
         <p>Potenza: <span>150</span>CV | <span>110</span>kW </p>
        </div>
        <div class="cilindrata">
         <p>Cilindrata: <span>1395</span> cm <sup>3</sup> </p>
        </div>
       </div>
       <div class="tpc-btn">
        <button :style="{color: car.color1, border: 1 +'px' + ' '+ 'solid' + ' ' + car.color1, width: 10.5+'rem', height: 4+'rem'}" v-html="car.btnText" > </button>
       </div>
      </div>
      <div class="distances" >
       <div class="distance1">
        <div class="number-text-icon">
         <div class="distance1-number" :style="{color: car.color1}"> {{car.distance1}} </div>
         <div class="distance1-text"> {{car.distance1Text}} </div>
         <div class="distance1-icon"><i class="fa fa-info" aria-hidden="true"></i></div>
        </div>
        <div class="distance1-illustration">
         <div class="illu1 distance1-illuBg1" > <!--:style="{background: car.color1}"-->
          <div id="dist1-1stdiv-left" :style="{width: car.dist1Illu1ColoredWidth , background: car.color1}"></div>
          <div id="dist1-1stdiv-right"></div>
         </div>
         <div class="illu1 distance1-illuBg">
          <div id="dist1-2nddiv-left" :style="{width: car.dist1Illu2ColoredWidth , background: car.color1}"></div>
          <div id="dist1-2nddiv-right"></div>
         </div>
         <div class="illu1"></div>
         <div class="illu1"></div>
         <div class="illu1"></div>
         <div class="illu1"></div>
        </div>
        
       </div>

       <div class="distance2" v-show="car.distance2">
        <div class="number-text-icon">
         <div class="distance2-number" :style="{color: car.color2}"> {{car.distance2}} </div>
         <div class="distance2-text"> {{car.distance2Text}}</div>
         <div class="distance2-icon"><i class="fa fa-info" aria-hidden="true"></i></div>
        </div>
        <div class="distance2-illustration">
         <div class="illu2 distance2-illuBg1" > <!--:style="{background: car.color1}"-->
          <div id="dist2-1stdiv-left" :style="{width: car.dist2Illu1ColoredWidth , background: car.color2}"></div>
          <div id="dist2-1stdiv-right"></div>
         </div>
         <div class="illu2 distance2-illuBg">
          <div id="dist2-2nddiv-left" :style="{width: car.dist2Illu2ColoredWidth , background: car.color2}"></div>
          <div id="dist2-2nddiv-right"></div>
         </div>
         <div class="illu2"></div>
         <div class="illu2"></div>
         <div class="illu2"></div>
         <div class="illu2"></div>
        </div>
        
       </div>
      </div>
     </div>



     <!-- <div class="car">
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
         <div class="distance1-icon"><i class="fa fa-info" aria-hidden="true"></i></div>
        </div>
        <div class="distance1-illustration">
         <div class="illu1" id="distance1-illuBg"></div>
         <div class="illu1"></div>
         <div class="illu1"></div>
         <div class="illu1"></div>
         <div class="illu1"></div>
         <div class="illu1"></div>
        </div>
        
       </div>

       <div class="distance2">
        <div class="number-text-icon">
         <div class="distance2-number">6,81</div>
         <div class="distance2-text">€x100km col cor. alternata</div>
         <div class="distance2-icon"><i class="fa fa-info" aria-hidden="true"></i></div>
        </div>
        <div class="distance2-illustration">
         <div class="illu2" id="distance2-illuBg"></div>
         <div class="illu2" id="illu2-divided">
           <div class="illu2-colored"></div>
           <div class="illu2-uncolored"></div>
         </div>
         <div class="illu2"></div>
         <div class="illu2"></div>
         <div class="illu2"></div>
         <div class="illu2"></div>
        </div>
        
       </div>
      </div>
     </div> -->
    </div>
    <div class="carica-btn">
      <button>CARICA ALTRE AUTO</button>
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
          id: 1,
          picture: 'images/vw-gray.jpg',
          model: 'VOLKSWAGEN ECO UP! <br>',
          type: 'move 5p',
          tipo: 'Berlina',
          potenza: '150CV | 110kW',
          cilindrata: '1395 cm',
          btnText: 'GPL',
          color1: '#005999',
          distance1: '3,85',
          distance1Text: '€x100km per le tue abitudini',
          dist1Illu1ColoredWidth: '85%',
          dist1Illu2ColoredWidth: '0px',
        },
        {
          id: 2,
          picture: 'images/ford.jpg',
          model: 'FORD FIESTA',
          type: '1.1 75 CV Gpl <br> 5p.',
          tipo: 'Berlina',
          potenza: '150CV | 110kW',
          cilindrata: '1395 cm',
          btnText: 'GPL',
          color1: '#005999',
          distance1: '4,96',
          distance1Text: '€x100km',
          dist1Illu1ColoredWidth: '100%',
          dist1Illu2ColoredWidth: '0px',
        },
        {
          id: 3,
          picture: 'images/hyunday.jpg',
          model: 'HYUNDAY IONIQ',
          type: 'ELECTRIC <br> EV 38.3 kWh',
          tipo: 'Berlina',
          potenza: '150CV | 110kW',
          btnText: 'ELECTTRICA',
          color1: '#009ee3',
          color2: '#95cfed',
          distance1: '3,40',
          distance1Text: '€x100km - ricarica domestica',
          distance2: '8,54',
          distance2Text: '€x100km - col. cor. continua',
          dist1Illu1ColoredWidth: '70%',
          dist1Illu2ColoredWidth: '0px',
          dist2Illu1ColoredWidth: '100%',
          dist2Illu2ColoredWidth: '70%',
        },
        {
          id: 4,
          picture: 'images/toyota.jpg',
          model: 'TOYOTA PRIUS',
          type: 'Plug-in <br> Hybrid',
          tipo: 'Berlina',
          potenza: '150CV | 110kW',
          cilindrata: '1395 cm',
          btnText: 'PLUG-IN <br> HYBRID',
          color1: '#009933',
          color2: '#88b31a',
          distance1: '5,11',
          distance1Text: '€x100km - ricarica domestica',
          distance2: '6,81',
          distance2Text: '€x100km - col. cor. alternata',
          dist1Illu1ColoredWidth: '100%',
          dist1Illu2ColoredWidth: '0px',
          dist2Illu1ColoredWidth: '100%',
          dist2Illu2ColoredWidth: '30%',
        },
        {
          id: 5,
          picture: 'images/toyota-blue.jpg',
          model: 'TOYOTA Prius 4a serie',
          type: '1.8 <br> AWD Lounge',
          tipo: 'Berlina',
          potenza: '150CV | 110kW',
          cilindrata: '1395 cm',
          btnText: 'FULL HYBRID',
          color1: '#009933',
          distance1: '6.97',
          distance1Text: '€x100km',
          dist1Illu1ColoredWidth: '100%',
          dist1Illu2ColoredWidth: '30%',
        },
        {
          id: 6,
          picture: 'images/toyota-light-blue.jpg',
          model: 'TOYOTA AYGO',
          type: '1.0 VVT-i 72 <br> CV 5p.',
          tipo: 'Berlina',
          potenza: '150CV | 110kW',
          cilindrata: '1395 cm',
          btnText: 'BENZINA',
          color1: '#e20000',
          distance1: '7,96',
          distance1Text: '€x100km',
          dist1Illu1ColoredWidth: '100%',
          dist1Illu2ColoredWidth: '30%',
        },
      ],
    }
  },
}
</script>

<style scoped>


#dist1-1stdiv-left, #dist1-1stdiv-right, #dist1-2nddiv-left, #dist1-2nddiv-right, #dist2-1stdiv-left, #dist2-1stdiv-right, #dist2-2nddiv-left, #dist2-2nddiv-right {
  height: 100%;
}
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
  border-radius: 0.6rem;
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
  z-index: 1;
}
#costo {
  color: rgb(250, 77, 46);
}

.fade-enter-from {
  opacity: 0;
}
.fade-enter-to {
  opacity: 1;
}
.fade-enter-active {
  transition:  opacity 500ms ease;
}
.fade-leave-from {
  opacity: 1;
}
.fade-leave-to {
  opacity: 0;
}
.fade-leave-active {
  transition: opacity 300ms ease;
}



.all-cars {
 /* border: 1px solid; */
 margin: 0 1rem;
}

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
 /* padding-bottom: 1rem; */
}
.model-title p {
 /* width: 80%; */
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
 margin: 1rem 0;
}
.div-with-btn p {
 text-align: left;
 font-size: 1rem;
 /* color: rgb(44, 44, 44); */
 color: rgba(49, 49, 49, 0.9)
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
 padding: 0.5rem 1.5rem;
 background-color: #fff;
}
.number-text-icon {
  display: flex;
  align-items: center;
  justify-items: center;
}
.distance1-number, .distance2-number {
  font-family: 'Work Sans', sans-serif;
  color: rgb(3, 145, 3);
  font-size: 2rem;
  font-weight: bold;
  margin-right: 0.5rem;
}

.distance1-icon, .distance2-icon {
  flex: 1;
  text-align: right;
  
}

.fa-info {
  color: #6e6e6ea9;
  border: 2px solid #6e6e6ea9;
  border-radius: 50%;
  padding: 0 0.35em;
}
.distance1-illustration, .distance2-illustration {
  display: flex;
  justify-content: space-between;
  margin: 1em 0;
}
.illu1, .illu2 {
  height: 0.6rem;
  /* border: 1px solid; */
  flex: 1;
  background-color: #e9e8e8;
  margin-right: 0.1em;
}


.carica-btn {
  /* border: 1px solid; */
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 2rem;
  margin-top: 2rem;
}
.carica-btn button {
  color: #fff; 
  background-color: rgb(250, 77, 46);
  width: 100%;
  border: 0;
  margin: 0 1rem;
  font-weight: bold;
  font-family: 'Work Sans', sans-serif;
  font-size: 1.05em;
  padding: 1rem;
  /* height: 100%; */
  /* font-family: ; */

}


</style>
