<template>
  <div id="app"  v-scroll="handleScroll" >
    <div class="row justify-content-end m-0  bg " >
      <div class="bg  position-fixed final justify-content-end  menuNav d-md-flex d-none align-items-center"  :class="{'navbar--hidden' : !shownav }">
            <div id="nav" class="row m-0 col-xl-5 col-ld-6 col-md-7 justify-content-between   align-items-center ">
              <a href="#nosotros">Nosotros</a>
              <a href="#soluciones">Soluciones</a>
              <a href="#Modelo">Modelo</a>
              <a href="#Equipo">Equipo</a>
              <a href="#Contacto">Contacto</a>
          </div>
      </div>
    </div>

  <!--Menu hamburguesa-->
    <div class="menu-h  d-md-none d-flex align-items-center " :class="{'navbar--hidden' : !shownav }">
        <button class="js-menu menu position-fixed" type="button" @click="activeAbrir()" @mouseout="cerrar()">
          <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" focusable="false" width="2em" height="2em" style="-ms-transform: rotate(360deg); -webkit-transform: rotate(360deg); transform: rotate(360deg);" preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24"><g fill="none"><path d="M4 6h16M4 12h16M4 18h16" stroke="#626262" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></g></svg>        
        </button>
    </div>
    <div  class="position-fixed navsitoD" :class="{'abrir-menu' : abrir}">
        <nav>
          <svg class="equis" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" focusable="false" width="1em" height="1em" style="-ms-transform: rotate(360deg); -webkit-transform: rotate(360deg); transform: rotate(360deg);" preserveAspectRatio="xMidYMid meet" viewBox="0 0 24 24"><g fill="none" stroke="#626262" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M18 6L6 18"/><path d="M6 6l12 12"/></g></svg>
          <div id="nav" class="row flex-column m-0">
              <a class="mt-2 mb-2"  href="#nosotros">Nosotros</a>
              <a class="mt-2 mb-2"  href="#soluciones">Soluciones</a>
              <a class="mt-2 mb-2"  href="#Modelo">Modelo</a>
              <a class="mt-2 mb-2"  href="#Equipo">Equipo</a>
              <a class="mt-2 mb-2"  href="#Contacto">Contacto</a>
          </div>
            <div class="redes-contacto-menu row flex-column">
                <a href="https://www.instagram.com/itprojectperu/" class="ml-1 mr-1 red-menu">
                   Instagram
                </a>
                <a href="https://www.facebook.com/Itprojectperu-101730618663668" class="ml-1 mr-1 red-menu">
                    Facebook
                </a>
                <a href="https://www.linkedin.com/company/itprojectperu/about/?viewAsMember=true" class="ml-1 mr-1 red-menu">
                    LinkedIn
                </a>
            </div>
      </nav>
    </div>
  


    <MenuHamburguesa/>
    <HelloWorld/>
    <Empoderamos style="padding-top:4rem;" id="nosotros"/>
    <MisionVision />
    <NuestrosValors />

        <div id="soluciones" class="row justify-content-end m-0" style="padding-top:4rem;">
             <h2 class="soluciones col-md-6 col-10 p-0" >NUESTRAS SOLUCIONES</h2>
        </div>
        <div class="card-grande d-none d-md-block d-lg-block">
            <div class=" d-flex justify-content-between align-items-center contenedor-animacion" >
              <div class="bacU d-flex m-0 justify-content-center align-items-center " @mouseover="agregarMove()" @mouseout="quitarMover()" :class=" [move ? 'crear' : '', moveD ? 'cerrar' : '']">
                  <div class="tama-uni p-0  row m-0 justify-content-between align-items-center w-100 "  :class="{mostrar : move }">
                    <Rodilla v-on:start="moveD" style="height:49rem; width:100%" :class="{dance: moveD}" class="fijo"/>
                  </div>
                  <div :class=" [move ? 'oculta' : '', moveD ? 'oculta' : '']" class="grande"><h1 class="fuente text-right fffz col-md-5 " style=" margin-right: 25rem;" >PRÓTESIS</h1></div>
              </div>

              <div class="backD d-flex m-0 justify-content-between align-items-center  p-0" @mouseover="agregarMoveD()" @mouseout="quitarMover()"  :class=" [moveD ? 'crear' : '', move ? 'cerrar' : '']">
                  <div  :class="  [move ? 'oculta' : '', moveD ? 'oculta' : '']" class="grande"><h1 class="fuente text-left fffz " >PROGRAMA DE EMPODERAMIENTO</h1></div>
                  <div class="tama-uniD p-0  d-flex m-0 justify-content-between align-items-center " :class="{mostrar : moveD }">
                    <ProgramaEmpoderamiento :class="{dance: move}" class="heisito" />
                  </div>
              </div>
            </div>
        </div>

    <Rodilla class="d-block d-md-none d-lg-none"/>
    <ProgramaEmpoderamiento  class="d-block d-md-none d-lg none"/>
    <NuestrasSoluciones />
    <NuestroModelo style="padding-top:4rem;" id="Modelo"/>
    <Beneficiados/>
    <div id="Equipo">
      <EquipoCarrusel class="d-block d-md-block d-lg-none my-5" />
      <Equipo class="d-none d-md-none d-lg-block" />
    </div>


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
import MenuHamburguesa from '@/components/MenuHamburguesa.vue'
import EquipoCarrusel from '@/components/EquipoCarrusel.vue'
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
    MenuHamburguesa,
    EquipoCarrusel,
    Footer
  },
  data() {
    return {
      move:false,
      moveD:false,
      guardarU:false,
      guardarD:false,
      llevar:false,
      llevarD:false,
      abrir:false,
      lastScrollPosition: 0,
      shownav:true
  }
  },
  mounted () {
    this.lastScrollPosition = window.scrollY
  },

  methods: {



  handleScroll: function (evt, el) {
    var currentScrollPos = window.scrollY
    if (this.lastScrollPosition < currentScrollPos) {
      this.shownav = false
    } else {
      this.shownav = true
    }
    this.lastScrollPosition = currentScrollPos;
    },




    agregarMove(){
      this.move = true
      this.guardarD = true
      var that = this
      setTimeout(function(){ 
        that.llevar = true
        }, 500);
    },
     agregarMoveD(){
      this.moveD = true
      this.guardarU = true
      var that = this
      setTimeout(function(){ 
      that.llevarD = true
      }, 500);
    },
    quitarMover(){
       this.move = false
       this.moveD = false
       this.guardarU = false
       this.guardarD = false
        this.llevar = false
       this.llevarD = false
      },
      activeAbrir(){
        this.abrir = ! this.abrir
      },
      cerrar(){
        this.abrir = false
      }
    }
}
</script>
<style>
    html {
        scroll-behavior: smooth;
    }
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
     @font-face {
      font-family: 'Aileron-SemiBold';
      src: url('./assets/fuente/aileron/Aileron-SemiBold.otf') 
  }
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #424242;
  max-width: 120rem;
  margin: 0 auto;
  overflow-x: hidden;
}



#nav a {
  font-family: 'QuireSansBold';
  color: #424242;
  font-size: 0.9rem
}

#nav a.router-link-exact-active {
  color: #42b983;
}
.fuente{
  font-family: 'Kollektif';
  color: #ffffff;
  width: 100%;
  width: 33rem
}
.fuente::after{
    content: '';
    display: block;
    height: 0.2rem;
    width: 100%;
    background-color:   #fff;
    }
  .soluciones{
    font-size: 2.8rem;
    padding: 0;
    border-bottom: rgb(63, 63, 63) 3px solid;
    margin-bottom: 4rem;
  }
.nuestros{
  color: #424242;
}
.bacU{
  background:#3755E0;
  width: 50%;
  height: 49rem;
  transition: width 1s;
}
.backD{
  background:#DD3B00;
  width: 50%;
  height: 49rem;
  padding: 0rem 1rem;
  transition: width 1s;
}

.crear{
  width: 100%;
  transition: width 1s;
}

.cerrar{
  width: 5%;
}
.oculta{
  transform: scale(0);
  transition: 0.5s ease;
  transition: width 1s;
  width: 0%!important;
  margin:0!important; 
}

.grande{
  width: 100%;
   margin-left: 8rem;
}

.fffz{
  padding: 0 3rem;
  transition: 0.5s ease;
}
.tama-uni{
  transform: translate(-140%);
  transition: 0.5s ease;
}
.mostrar{
  transform: translate(0)!important;
  transition: 1s ease;
}
.tama-uniD{
  transform: translate(100%);
  transition: 0.5s ease;
}
.dance{
  transition: 1.5s ease;
  opacity: 0!important;
}
.equis{
    position: absolute;
    right: 1rem;
    width: 2rem;
    height: 1.5rem;
    top: 1rem;
}

.bg{
  background: #ffffff;
      z-index: 9;
}
.final{
  right: 0rem;
  width: 101%
}
.fijo{
   transition: 1s ease;
   opacity: 1
}
.menuNav {
  height: 60px;
  width: 100vw;
  position: fixed;
  transform: translate3d(0, 0, 0);
  transition: 0.1s all ease-out;
}
.menuNav.navbar--hidden {
  box-shadow: none;
  transform: translate3d(0, -100%, 0);
}
.navbar--hidden {
  box-shadow: none;
  transform: translate3d(0, -100%, 0);
}
.heisito{
  height:49rem
}
.red-menu{
  font-family: aileron-bold;
  text-decoration: revert;
}
/*Menu Hamburguesa */

.abrir-menu{
  transition: all 0.5s ease;
  transform: translateX(10px);
  z-index: 9;
  right: 0rem!important;
  top:0;
  display: flex;
  flex-direction: column;
  justify-content:space-between
}
.menu-h{
    position: fixed;
    z-index: 9;
    background: #ffffff;
    width: 100%;
    height: 4rem;
}
.menu {
  background: transparent;
  margin: 0;
  width: 45px;
  height: 40px;
  z-index: 1;
  outline: 0;
  border: 0;
  z-index: 999!important;
  background-color: #fff;
  border-radius:5px;
  right: 1rem;
}

.bar, .bar::before, .bar::after {
  transition: 0.2s background linear 0.1s, 0.2s top linear 0.2s, 0.2s -webkit-transform linear;
  transition: 0.2s background linear 0.1s, 0.2s top linear 0.2s, 0.2s transform linear;
  transition: 0.2s background linear 0.1s, 0.2s top linear 0.2s, 0.2s transform linear, 0.2s -webkit-transform linear;
  margin: auto;
  width: 100%;
  height: 0.2rem;
  content: '';
  top: 50%;
  left: 0;
}
.bar::before {
  top: -0.7rem;
}
.bar::after {
  top: 0.7rem;
}
.bar::before, .bar::after {
  -webkit-transform: rotate(0deg);
          transform: rotate(0deg);
}
.active .bar {
  background: 0;
}
.active .bar::before {
  -webkit-transform: rotate(45deg);
          transform: rotate(45deg);
}
.active .bar::after {
  -webkit-transform: rotate(-45deg);
          transform: rotate(-45deg);
}
.active .bar::before, .active .bar::after {
  top: 0;
}
.active .bar, .active .bar::before, .active .bar::after {
  transition: 0.2s background linear 0.1s, 0.2s top linear, 0.2s -webkit-transform linear 0.2s;
  transition: 0.2s background linear 0.1s, 0.2s top linear, 0.2s transform linear 0.2s;
  transition: 0.2s background linear 0.1s, 0.2s top linear, 0.2s transform linear 0.2s, 0.2s -webkit-transform linear 0.2s;
}

.navsitoD {
    height: 100%;
  z-index: 9999;
  right: -40rem;
    transition: all 0.5s ease;

}
nav{
  display: flex!important;;
  flex-direction: column;
  justify-content: space-between;
  background: #F7E200!important;
  color: #424242;
  font-size: 10px;
  width: 200px;
  height: 100%;
  transition: all 0.5s ease;
  padding-top: 20px;
}
.menu-open nav {
  -webkit-transform: translateX(0);
          transform: translateX(0);
}
#HTML2 li {display: flex;align-items: center;}

nav ul {
  margin: 0;
  list-style: none;
  padding: 0;
}

nav {
    padding: 40px;
    margin: 0;
}
nav h2{
  font-size: 24px;
  margin-bottom: 10px;
}
nav span {
  margin-bottom: 20px;
}
nav ul{
    margin-top: 20px
}
nav ul li, nav span {
  font-size: 14px;height: 40px;
}
nav ul li{
    border-bottom: 1px solid;
}
nav li i{
  margin-right: 5px; font-size: 20px!important;
}
.redes-menu{
  width: 2rem
}
.redes-contacto-menu {
  right: 1rem;
  color: #424242;
   font-family: 'Kollektif-Bold';
}
a{
    color: #424242!important;
}
@media only screen and (max-width: 320px){
  
      .soluciones{
        margin-left: 0rem;
        padding: 0;
        margin-bottom: 4rem;
        font-size: 2rem;
        border-bottom: rgb(63, 63, 63) 3px solid;
    }
} 
  @media only screen and (max-width: 426px) and (min-width: 321px){
    
      .soluciones{
        margin-left: 0rem;
        padding: 0;
        margin-bottom: 4rem;
        font-size: 2rem;
        border-bottom: rgb(63, 63, 63) 3px solid;
    }
  }

  @media only screen and (max-width: 600px) and (min-width: 425px) {
        
      .soluciones{
        margin-left: 0rem;
        padding: 0;
        margin-bottom: 4rem;
        font-size: 2rem;
        border-bottom: rgb(63, 63, 63) 3px solid;
    }
  }
  @media only screen and (max-width: 768px) and (min-width: 601px){
      .crear {
        width: 95%;
        transition: width 1s;
    }
    .heisito{
      height:100%
    }
    .grande{
      width: 100%;
      margin-left: 2rem;
  }
        .soluciones{
        margin-left: 0rem;
        padding: 0;
        margin-bottom: 4rem;
        font-size: 2rem;
        border-bottom: rgb(63, 63, 63) 3px solid;
    }
  }
  @media only screen and (max-width: 1204px) and (min-width: 769px) {
    .grande {
      width: 100%;
      margin-left: 0rem;
  }

    }
</style>
