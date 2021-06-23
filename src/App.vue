<template>
  <div id="app">
    <div id="webglcontainer"></div>
    <div id="preloader" class="preloader">
        <div id="preloaderBar" class="vAligned">
            Caricando del drip
            <div class="preloaderBorder">
                <div id="preloaderProgress" class="preloaderProgress">
                </div>
            </div>
        </div>
    </div>
    <div id="errorContainer" class="vAligned hidden">
        <p id="errorMessage"></p>
    </div>
    <div id="playContainer" class="vAligned hidden">
       
    </div>
    
    <div class="text">
      <h1>UN MARE <br> DI <span style="filter:blur(3px);">GUAI</span></h1>
      <p><a target="_blank"  style="color : #cccccc;" href="https://instagram.com/naive.17">NAIVE</a> x <a target="_blank" href="https://instagram.com/relliadeus" style="color : #cccccc;">RELLIADEUS</a></p>
      <pre>/haɪˈpɜːrbəli/</pre>
      <p>"Ti sei cacciato in un mare di guai piccolo naive"</p>
      <p>- Relliadeus che decide di fare una collaborazione con Naive, che dice "ao famo la scritta GUAI che sta nel mare ma la famo in javascript letteralmente zi"</p>
 
      <p style="font-size : 14px;"> Simulazione liquida particellare</p>
    </div>
    
    <div class="tipregousaundesktopfra">

      <p>Ridimensiona la finestra ad almeno 1400 x 800</p>

    </div>

  </div>
</template>

<script>
//import SPH from "./components/sph.js";

export default {
  name: 'App',
  data(){
    return {
      //SPH
    }
  },
  components: {
  },
  mounted(){
  }
}
</script>

<style>
@font-face {
    font-family: "Voyage-Regular";
    font-display: swap;
    src: url("/assets/Voyage-Regular.ttf");
    font-style: normal;
}


@font-face {
    font-family: 'Helvetica Neue LT Std';
    src: url('/assets/HelveticaNeueLTStd-Lt.woff2') format('woff2'),
        url('/assets/HelveticaNeueLTStd-Lt.woff') format('woff');
    font-weight: 300;
    font-style: normal;
    font-display: swap;
}



.hidden {
    display: none;
}
.preloader {
    position: fixed;
    height: 100vh;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    vertical-align: middle;
    background: black;
    display: flex;
    flex-flow: column;
    justify-content: center;
    align-items: center;
    z-index: 99999999;
}

.preloaderBorder {
    margin-top: 10px;
    width: 300px;
    height: 2px;
    padding: 2px;
}

.preloaderProgress  {
    width: 0%;
    height: 100%;
    background: white;
}

#app {
  display : fleX;
  flex-flow : row;
  background-color : black;
  color : white;
  font-family: "Helvetica Neue LT Std";
  overflow : hidden;
}

html, body {
  background-color : black;
  margin : 0px;
  overflow : hidden;
}

.text {
  color : #cccccc;
  display: flex;
  flex-flow : column;
  justify-content: center;
  z-index: 1;
  position : relative;
  padding : 60px;
  font-weight: 100;
}

h1 {
  font-size : 120px;
  margin-top : 0px;
  margin-bottom : 0px;
  margin-left : -8px;
}

p {
  margin-top : 0px;
}

.tipregousaundesktopfra {
  display : none;
}

@media screen and (max-width : 1400px) {
  .tipregousaundesktopfra {
    display : flex;
    position : fixed;
    top : 0px;
    left: 0px;
    width : 100vw;
    height : 100vh;
    background-color : black;
    color : #aaaaaa;
    flex-flow : row;
    z-index: 99999999999999999999;
    justify-content: center;
    align-items: center;
  }
}
</style>
