<template>
  <div class="footer">
    <div class="quattroruote">
      <h2>QUATTRORUOT<span>e</span></h2>
    </div>
    <div class="sitemap-contatti-redazione">
      <div class="sitemap">Sitemap</div>
      <div class="contatti">Contatti</div>
      <div class="redazione">Redazione</div>
    </div>
    <div class="socials">
      <i class="fa fa-youtube-play" aria-hidden="true"></i>
      <i class="fa fa-facebook" aria-hidden="true"></i>
      <i class="fa fa-twitter" aria-hidden="true"></i>
      <i class="fa fa-instagram" aria-hidden="true"></i>
      <i class="fa fa-rss" aria-hidden="true"></i>
    </div>
    <div class="footer-text">
      <p>
        Editoriale Domus SpA Via G. Mazzocchi, 1/3 20089 Rozzano (Mi) - Codice
        fiscale, partita IVA e iscrizione al Registro delle Imprese di Milano n.
        07835550158 R.E.A. di Milano n. 1186124 - Capitale sociale versato €
        5.000.000,00 - Tutti i diritti riservati - All rights reserved -
        Informativa Privacy - Informativa Cookie completa - Lic. SIAE n.
        4653/I/908
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Footer',
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Biryani:wght@900&family=Kanit:wght@800&display=swap');

.footer {
  background-color: #292929;
  grid-column: 1 / -1;
  padding-bottom: 4rem;
}
.quattroruote {
 margin-top: 2rem;
}
.quattroruote h2 {
  color: #fff;
  /* font-family: 'Kanit', sans-serif; */
  /* font-family: 'Balsamiq Sans', cursive; */
  /* letter-spacing: 0em; */
  font-family: 'Biryani', sans-serif;
  /* font-family: 'Kanit', sans-serif; */
  /* border: 1px solid; */
}
.quattroruote h2 span {
  font-size: 1.8rem;
}
.sitemap-contatti-redazione {
  display: flex;
  justify-content: center;
  align-items: center;
  /* border: 1px solid; */
}
.sitemap,
.contatti,
.redazione {
  color: #c1c1c1;
  margin: 0.5rem 0;
  padding: 0 0.5rem;
}
.sitemap,
.contatti {
  border-right: 1px solid #c1c1c1;
}
.socials {
  /* border: 1px solid red; */
  width: 40%;
  margin: 1rem auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.fa {
  color: #d6d6d6;
  font-size: 1.5rem;
}
.footer-text {
  margin: 1rem;
  border-top: 1px solid #d6d6d6;
  padding-top: 1rem;
}
.footer-text p {
 color: #d6d6d6;
 font-size: 0.7rem;
 line-height: 1.1rem;
}
</style>
