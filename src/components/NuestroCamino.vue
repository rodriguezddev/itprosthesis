<template>
    <div class="cont-camino" :style="'background:'+ colorsito">
        <h2 class="nuestros col-md-5 camnino col-8 ">NUESTRO CAMINO</h2>
        <div class="row m-0 justify-content-around flex-md-column flex-lg-row flex-column ccc">
            <div class=" position-absolute linea "></div>
            <div class="row flex-column align-items-center mt-3" @mouseover="cambiars(ids[0])" @mouseout="volver()">
                <div class="circle">
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 211 211"><defs></defs><g id="Capa_2" data-name="Capa 2"><g id="Capa_4" data-name="Capa 4"><polyline class="cls-check" points="51.96 113.05 95.47 148 170 57.94"/><circle class="cls-check" cx="105.5" cy="105.5" r="103"/></g></g></svg>
                </div>
                <div class="izquierda">
                    <p class="color-camino">Identificación de necesidades</p>
                    <p class="color-camino">2020 - 1</p>
                </div>
            </div>
            
            <div class="row flex-column align-items-center mt-3" @mouseover="cambiars(ids[1])" @mouseout="volver()">
                <div class="circle">
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 211 211"><defs></defs><g id="Capa_2" data-name="Capa 2"><g id="Capa_4" data-name="Capa 4"><polyline class="cls-check" points="51.96 113.05 95.47 148 170 57.94"/><circle class="cls-check" cx="105.5" cy="105.5" r="103"/></g></g></svg>
                </div>
                <div class="derecha">
                    <p class="color-camino">Diseño conceptual</p>
                    <p class="color-camino">2020 - 2</p>
                </div>
            </div>
            
            <div class="row flex-column align-items-center mt-3" @mouseover="cambiars(ids[2]),  agg()" @mouseout="volver()">
                <div class="circle color-uno-d">
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 211 211"><defs></defs><g id="Capa_2" data-name="Capa 2"><g id="Capa_4" data-name="Capa 4"><polyline class="cls-rojo" points="51.96 113.05 95.47 148 170 57.94"/><circle class="cls-rojo" cx="105.5" cy="105.5" r="103"/></g></g></svg>
                </div>
                <div class="izquierda ">
                    <p class="color-camino chanD" :class="{chanDes : show}">Materialización</p>
                    <p class="color-camino chanD" :class="{chanDes : show}">2021</p>
                </div>
            </div>
            
            <div class="row flex-column align-items-center mt-3" @mouseover="cambiars(ids[3]),  agg()" @mouseout="volver()">
                <div class="circle color-dos-d">
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 211 211"><defs></defs><g id="Capa_2" data-name="Capa 2"><g id="Capa_4" data-name="Capa 4"><polyline class="cls-azul" points="51.96 113.05 95.47 148 170 57.94"/><circle class="cls-azul" cx="105.5" cy="105.5" r="103"/></g></g></svg>
                </div>
                <div class="derecha ">
                    <p class="color-camino chan" :class="{chanDes : show}">Primeras ventas</p>
                    <p class="color-camino chan" :class="{chanDes : show}">2021</p>
                </div>
            </div>
            
            <div class="row flex-column align-items-center mt-3" @mouseover="cambiars(ids[4])" @mouseout="volver()">
                <div class="circle"></div>
                <div class="izquierda">
                    <p class="color-camino">Indrustrializacion</p>
                    <p class="color-camino">2022</p>
                </div>
            </div>
            
        </div>
    </div>
</template>
<script>
export default {
    name:'NuestroCamino',
    data() {
        return {
            colorsito:'#7B7B7B',
            ids:[0,1,2,3,4],
            colores:['#7B7B7B', '#7B7B7B', '#DD3B00', '#3755E0', '#7B7B7B', '#7B7B7B'],
            show:false
        }
    },
    methods:{
        cambiars(index){
            this.colorsito = this.colores[index]
            
        },
        agg(){
            this.show = true
        },
        volver(){
            this.colorsito = '#7B7B7B'
            this.show = false
        }
    }
}
</script>
<style>
    .cls-check{
        fill:none;
        stroke: #ffffff;;
        stroke-linecap:round;
        stroke-miterlimit:10;
        stroke-width:5px;
    }
    .cls-rojo{
        fill:none;
        stroke: #DD3B00;;
        stroke-linecap:round;
        stroke-miterlimit:10;
        stroke-width:5px;
    }
     .cls-azul{
        fill:none;
        stroke: #3755E0;;
        stroke-linecap:round;
        stroke-miterlimit:10;
        stroke-width:5px;
    }
    .cont-camino{
        background-color: #7B7B7B;
        width: 100%;
        padding: 3rem 0rem;
        transition: 0.4s all ease;
    }
    .camnino{
        color: #fff;
        font-size: 2rem;
    }
    .camnino::after{
        content: '';
        display: block;
        height: 0.2rem;
        width: 24rem;
        background-color: #fff;
    }
    .circle{
        width: 5rem;
        height: 5rem;
        border-radius:100%;
        border:solid 4px #fff;
        background-color: #7B7B7B;
        position: relative;
    }
    .linea{
        border-top:solid 4px #fff;
        z-index: 0;
        margin-top: 3.5rem;
        width: 100%;
    }
    .color-camino{
        color: #fff;
        margin: 0;
        font-weight: bold;
        text-align: center;
    }
    .color-uno-d{
        border:solid 4px #DD3B00!important;
        background-color: #7B7B7B;
    }
    .color-dos-d{
        border:solid 4px #3755E0!important;
        background-color: #7B7B7B;
        color: #3755E0
    }
    .chanD{
        color: #DD3B00!important;
    }
    .chan{
        color: #3755E0!important;
    }
    .chanDes{
        color: #fff!important;
    }
    @media only screen and (max-width: 600px){ 
      .linea{
        border-left:solid 4px #fff;
        z-index: 0;
        margin-top: 2.5rem;
        width: 0.1rem!important;
        height: 100%;
        left: 50%;
    }
    .camnino::after {
        content: '';
        display: block;
        height: 0.2rem;
        width: 15rem;
        background-color: #fff;
    }
    .tam-equema {
        height: 22rem;
        width: 22rem;
        position: absolute;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-between;
        margin-left: -3rem;
        margin-top: -3rem;
    }
    .borde-animacion {
        width: 17rem;
        height: 17rem;
        border: dashed #fff;
        border-radius: 100%;
    }
    .texto-centro {
        color: #fff;
        font-size: 1.3rem;
        font-weight: 700;
        transition: 1s all ease;
    }
}
@media only screen and (max-width: 768px) {
      .linea{
        border-left:solid 4px #fff;
        z-index: 0;
        margin-top: 0.5rem;
        left: 50%;
        width: 0.1px;
        height: 100%;
    }
    .circle{
        width: 12rem;
        height: 12rem;
        border-radius:100%;
        border:solid 4px #fff;
        background-color: #7B7B7B;
        position: relative;
    }
    .derecha {
        position: absolute;
        margin-top: 5rem;
    }
    .izquierda {
        position: absolute;
        margin-top: 5rem;
    }
    .color-camino {
        color: #fff;
        margin: 0;
        font-weight: bold;
        text-align: center;
        width: 13rem;
    }
    
}
@media only screen and (max-width: 1024px) {
      .linea{
        border-left:solid 4px #fff;
        z-index: 0;
        margin-top: 0.5rem;
        left: 50%;
        width: 0.1px;
        height: 100%;
    }
    .circle{
        width: 12rem;
        height: 12rem;
        border-radius:100%;
        border:solid 4px #fff;
        background-color: #7B7B7B;
        position: relative;
    }
    .derecha {
        position: absolute;
        margin-top: 5rem;
    }
    .izquierda {
        position: absolute;
        margin-top: 5rem;
    }
    .color-camino {
        color: #fff;
        margin: 0;
        font-weight: bold;
        text-align: center;
        width: 13rem;
    }
    
}
</style>