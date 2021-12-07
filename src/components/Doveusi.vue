<template>
<transition name="doveUziFade">
  <div class="doveusi">
    <div class="doveusi-header">
      <div id="ex100kmlogo">
        <img src="images/ex100kmDove.jpg" alt="" />
      </div>
      <div id="ex100kmclose">
        <img src="images/closeex100km.jpg" alt="" @click="$emit('closeDoveUsi')"/>
      </div>
    </div>
    <div class="dove-usi-text">
      <h1 class="dove-usi-h1">Dove usi l'auto?</h1>
      <p class="dove-usi-p">
        Utilizza i
        <span style="color: rgb(250, 77, 46)"> <b>cursori</b></span> per
        modificare le percentuali relative al tipo di percorso che fai
        abitualmente, una volta impostati i valori clicca su Ricalcola
      </p>
    </div>
  </div>
  </transition>
</template>

<script>
export default {
  name: 'Doveusi',
  emits: ['closeDoveUsi']
}
</script>

<style scoped>
.doveusi {
  grid-column: 1 / -1;
  position: fixed;
  top: 0;
  width: 100%;
  /* height: 100%; */
  bottom: 0;
  z-index: 2;
  background: red;
}
.doveusi-header {
  display: flex;
  justify-content: space-between;
  /* align-items: center; */
  background: #fff;
}
.doveUziFade-enter-from {
 opacity: 0;
}
.doveUziFade-enter-to {
 opacity: 1;
}
.doveUziFade-enter-active {
 transition: opacity 300ms ease;
}
.doveUziFade-leave-from {
 opacity: 1;
}
.doveUziFade-leave-to {
 opacity: 0;
}
.doveUziFade-leave-active {
 transition: opacity 300ms ease;
}
#ex100kmclose {
 cursor: pointer;
}
</style>
