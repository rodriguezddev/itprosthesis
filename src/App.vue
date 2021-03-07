<template>
  <div id="app">
    <div class="row justify-content-end m-0">
      <div id="nav" class="row m-0 col-xl-5 col-ld-6 col-md-7 justify-content-between">
        <a href="#nosotros">Nosotros</a>
        <a href="#soluciones">Soluciones</a>
        <a href="#Modelo">Modelo</a>
        <a href="#Equipo">Equipo</a>
        <a href="#Contacto">Contacto</a>
      </div>
    </div>
    <HelloWorld/>
    <Empoderamos id="nosotros"/>
    <MisionVision id="soluciones"/>
    <NuestrosValors id="Modelo"/>
    <NuestrasSoluciones/>
      <div class="row justify-content-end m-0">
             <h2 class="nuestros col-md-5">NUESTRAS SOLUCIONES</h2>
        </div>
    <div class=" row m-0 justify-content-between align-items-center contenedor-animacion" :class="">

       <div class="bacU row m-0 justify-content-center align-items-center" @mouseover="agregarMove()" @mouseout="quitarMover()" :class=" [move ? 'moveU' : 'moveD', guardarU ? 'guardarU' : '']">
          <div class="tama-uni col-md-7 p-0  row m-0 justify-content-start align-items-center">
             <Rodilla class="col-md-12 p-0"/>
          </div>
         
           <div class="col-md-4"><h1 class="fuente text-center">PRÓTESIS</h1></div>
      </div>


      <div class="backD row m-0 justify-content-between align-items-center" @mouseover="agregarMoveD()" @mouseout="quitarMover()"  :class=" [moveD ? 'moveT' : 'moveC', guardarD ? 'guardarD' : '']">
          <div class="col-md-3"><h1 class="fuente text-center">PROGRAMA DE EMPODERAMIENTO</h1></div>
          <div class="tama-uni col-md-8 p-0">
             <ProgramaEmpoderamiento class="col-md-9"/>
          </div>
         
      </div>

    </div>
    <NuestroModelo/>
    <Beneficiados/>
    <Equipo id="Equipo"/>
    <CargosNegro/>
    <Contacto id="Contacto"/>
    <NuestroCamino/>
    <Footer/>
  </div>
</template>
<script>
import Empoderamos from '@/components/Empoderamos.vue'
import MisionVision from '@/components/MisionVision.vue'
import NuestrosValors from '@/components/NuestrosValors.vue'
import HelloWorld from '@/components/HelloWorld.vue'
import NuestrasSoluciones from '@/components/NuestrasSoluciones.vue'
import NuestroModelo from '@/components/NuestroModelo.vue'
import Beneficiados from '@/components/Beneficiados.vue'
import Equipo from '@/components/Equipo.vue'
import CargosNegro from '@/components/CargosNegro.vue'
import Contacto from '@/components/Contacto.vue'
import NuestroCamino from '@/components/NuestroCamino.vue'
import Rodilla from '@/components/Rodilla.vue'
import ProgramaEmpoderamiento from '@/components/ProgramaEmpoderamiento.vue'
import Footer from '@/components/Footer.vue'
export default {
  name:'App',
  components:{
    Empoderamos,
    MisionVision,
    NuestrosValors,
    HelloWorld,
    NuestrasSoluciones,
    NuestroModelo,
    Beneficiados,
    Equipo,
    CargosNegro,
    Contacto,
    NuestroCamino,
    Rodilla,
    ProgramaEmpoderamiento,
    Footer
  },
  data() {
    return {
      move:false,
      moveD:false,
      guardarU:false,
      guardarD:false,
      sobrepo:false
    }
  },
  methods:{
    agregarMove(){
      this.move = true
      this.guardarD = true
      console.log(this.move)
    },
     agregarMoveD(){
      this.moveD = true
      this.guardarU = true
      console.log(this.move)
    },
    quitarMover(){
       this.move = false
       this.moveD = false
       this.guardarU = false
       this.guardarD = false
      }
    }
}
</script>
<style>
    @font-face {
      font-family: 'Kollektif';
      src: url('./assets/fuente/kollektif/Kollektif.ttf') 
  }
    @font-face {
      font-family: 'Kollektif-Bold';
      src: url('./assets/fuente/kollektif/Kollektif-Bold.ttf') 
  }
    @font-face {
      font-family: 'Kollektif-BoldItalic';
      src: url('./assets/fuente/kollektif/Kollektif-BoldItalic.ttf') 
  }
    @font-face {
      font-family: 'Kollektif-Italic';
      src: url('./assets/fuente/kollektif/Kollektif-Italic.ttf') 
  }
  /*Quire*/
    @font-face {
      font-family: 'QuireSansBold';
      src: url('./assets/fuente/quire-sans-cufonfonts/QuireSansBold.ttf') 
  }
  /*aileron*/
    @font-face {
      font-family: 'aileron';
      src: url('./assets/fuente/aileron/Aileron-Thin.otf') 
  }
    @font-face {
      font-family: 'Aileron-Bold';
      src: url('./assets/fuente/aileron/Aileron-Bold.otf') 
  }
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #000;
  max-width: 120rem;
  margin: 0 auto;
  overflow-x: hidden;
}

#nav {
  padding: 30px 30px 15px 30px;
}

#nav a {
  font-family: 'QuireSansBold';
  color: #000;
  font-size: 0.9rem
}

#nav a.router-link-exact-active {
  color: #42b983;
}
.fuente{
  font-family: 'Kollektif-Bold';
  color: #ffffff;
  margin-left: 10rem;
}
.bacU{
  background:#3755E0;
  width: 152rem;
}
.backD{
  background:#DD3B00;
  width: 184rem;
}
.moveU{
  transform: translate(-5%);
  transition: all ease 0.5s;
}
.moveD{
    transform: translate(-68%);
    transition: all ease 0.5s;
}
.moveT{
  transform: translate(-134%);
  transition: all ease 0.5s;
}
.moveC{
    transform: translate(-75%);
    transition: all ease 0.5s;
}
.guardarU{
    transform: translate(-94.5%);
    transition: all ease 0.5s;
}
.guardarD{
    transform: translate(-54%);
    transition: all ease 0.5s;
}
.sobre{
  position: relative;
  z-index: 1;
}
.contenedor-animacion{
  width: 370rem;
}
</style>
