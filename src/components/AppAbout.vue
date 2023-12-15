<script>
export default {
  name: "AppContact",
};
</script>

<template lang="">
  <div id="about" class="d-flex justify-content-center align-items-center">
    <div class="container py-5">
      <div class="row">
        <div class="col-12 text-center">
          <h2 class="section">About Me</h2>
        </div>
        <div class="col-12 col-md-6">
          <p class="py-5">
            Ciao, sono Alessandro Iacovella, nato a Roma nel 1995. Sono un
            giovane Jr Full Stack Web Developer con un background nell'ambito
            della sociologia e criminologia, ottenuto con i miei studi
            universitari. <br />
            Appassionato e altamente motivato nel campo della programmazione.
            Dimostro un impegno costante nel migliorare le mie abilità tecniche
            e sono sempre alla ricerca di nuove sfide per ampliare il mio
            bagaglio professionale.<br />
            Mi sento molto a mio agio a lavorare in team, capacità acquisita
            durante tutto il mio percorso di studi e sento di poter dare spesso
            un parere positivo e contributi attivi poiché sono una persona
            socievole e collaborativa.
            <br />
          </p>
        </div>
        <div class="col-12 col-md-6">
          <div class="text-center py-5">
            <img
              src="../assets/images/AlessandroIacovella.jpg"
              alt="Foto-Profilo"
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
#about {
  background-color: rgb(20, 20, 20);
  color: white;
  padding-top: 50px;
  min-height: 100vh;
  img {
    height: 60%;
    width: 60%;
  }
}
</style>
