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
    <Rodilla/>
    <NuestrasSoluciones/>
    <ProgramaEmpoderamiento/>
    <NuestroModelo/>
    <Beneficiados/>
    <Equipo id="Equipo"/>
    <CargosNegro/>
    <Contacto id="Contacto"/>
    <NuestroCamino/>
    
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
    ProgramaEmpoderamiento
  }
}
</script>
<style>
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
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #000;
  font-size: 0.9rem
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
