<template>
    <div class="cont-camino" :class="colorsito">
        <h2 class=" col-md-5 camnino p-0 text-right col-8 " style=" font-family: 'Kollektif';">NUESTRO CAMINO</h2>
        <div class="row justify-content-around flex-md-row flex-lg-row flex-column ccc">
            <div class=" position-absolute lineax "></div>
            <div class="row flex-md-column align-items-center marginsito justify-content-around " @mouseover="cambiars(ids[0])" @mouseout="volver()">
                <div class="circle blanco">
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 211 211"><defs></defs><g id="Capa_2" data-name="Capa 2"><g id="Capa_4" data-name="Capa 4"><polyline class="cls-check" points="51.96 113.05 95.47 148 170 57.94"/><circle class="cls-check d-none d-md-block" cx="105.5" cy="105.5" r="103"/></g></g></svg>
                </div>
                <div class="izquierda p-0">
                    <p class="color-camino">Identificación de necesidades</p>
                    <p class="color-camino">2020 - 1</p>
                </div>
            </div>
            
            <div class="row flex-md-column align-items-center marginsito justify-content-around " @mouseover="cambiars(ids[1])" @mouseout="volver()">
                <div class="circle blanco">
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 211 211"><defs></defs><g id="Capa_2" data-name="Capa 2"><g id="Capa_4" data-name="Capa 4"><polyline class="cls-check" points="51.96 113.05 95.47 148 170 57.94"/><circle class="cls-check d-none d-md-block" cx="105.5" cy="105.5" r="103"/></g></g></svg>
                </div>
                <div class="derecha p-0">
                    <p class="color-camino">Diseño conceptual</p>
                    <p class="color-camino">2020 - 2</p>
                </div>
            </div>
            
            <div class="row flex-md-column align-items-center marginsito justify-content-around " @mouseover="cambiars(ids[2]),  agg()" @mouseout="volver()">
                <div class="circle  blanco color-uno-d" :class="{blanco : show}">
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 211 211"><defs></defs><g id="Capa_2" data-name="Capa 2"><g id="Capa_4" data-name="Capa 4"><polyline class="cls-rojo" points="51.96 113.05 95.47 148 170 57.94"/><circle class="cls-rojo d-none " cx="105.5" cy="105.5" r="103"/></g></g></svg>
                </div>
                <div class="izquierda  p-0">
                    <p class="color-camino chanD" :class="{chanDes : show}">Materialización</p>
                    <p class="color-camino chanD" :class="{chanDes : show}">2021</p>
                </div>
            </div>
            
            <div class="row flex-md-column align-items-center marginsito justify-content-around " @mouseover="cambiars(ids[3]),  agg()" @mouseout="volver()">
                <div class="circle blanco color-dos-d">
                </div>
                <div class="derecha  p-0">
                    <p class="color-camino chan" :class="{chanDes : show}">Primeras ventas</p>
                    <p class="color-camino chan" :class="{chanDes : show}">2021</p>
                </div>
            </div>
            
            <div class="row flex-md-column align-items-center marginsito justify-content-around " @mouseover="cambiars(ids[4])" @mouseout="volver()">
                <div class="circle blanco"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 211 211"><defs></defs><circle class="cls-check d-none d-md-block" cx="105.5" cy="105.5" r="103"/></svg></div>
                <div class="izquierda p-0">
                    <p class="color-camino">Industrialización</p>
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
            colorsito:'colorDinamicoU',
            ids:[0,1,2,3,4],
            colores:['colorDinamicoU', 'colorDinamicoU', 'colorDinamicoD', 'colorDinamicoT', 'colorDinamicoU', 'colorDinamicoU'],
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
            this.colorsito = 'colorDinamicoU'
            this.show = false
        }
    }
}
</script>
<style>
    .cls-check{
        fill:none;
        stroke: #7B7B7B;;
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
        background-color: #ffffff;
        width: 100%;
        padding: 3rem 0rem;
        transition: 0.4s all ease;
    }
    .camnino{
        font-size: 2.8rem;
        padding: 0;
        border-bottom: #fff 4px solid;
        color: #fff;
        margin-bottom: 3rem;
    }
    
    .circle{
        width: 5rem;
        height: 5rem;
        border-radius:100%;
        border:solid 4px  #fff;
        background-color: #fff;
        position: relative;
    }
    .lineax{
        border-top:solid 4px #ffffff;
        z-index: 0;
        margin-top: 3.5rem;
        width: 100%;
    }
    .color-camino{
        color: #ffffff;
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
    .blanco{
        background: #ffffff
    }
    .marginsito{
        margin-top: 1rem!important;
    }
    .colorDinamicoU{
        background: #7B7B7B
    }
    .colorDinamicoD{
        background: #DD3B00
    }
    .colorDinamicoT{
        background: #3755E0
    }
    @media only screen and (max-width:320px) {
                 .izquierda{
            flex: 0 0 41.666667%;
            max-width: 41.666667%;
        }
        .derecha{
            flex: 0 0 41.666667%;
            max-width: 41.666667%;
        }
            .lineax{
                border-left:solid 4px #7B7B7B;
                z-index: 0;
                margin-top: 2.5rem;
                width: 0.1rem!important;
                height: auto;
                left: 23%;
                min-height: 25rem;
            }
        .ccc{
            max-width: 84%;
            margin: 0 auto!important;
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
            .colorDinamicoU{
                background: #ffffff
            }
            .colorDinamicoD{
                background: #DD3B00
            }
            .colorDinamicoT{
                background: #3755E0
            }
               .circle{
                width: 5rem;
                height: 5rem;
                border-radius:100%;
                border:solid 4px  #7B7B7B;
                background-color: #fff;
                position: relative;
            }
                .color-camino{
                color: #7B7B7B;
                margin: 0;
                font-weight: bold;
                text-align: center;
            }
             .camnino{
                font-size: 2rem;
                padding: 0;
                border-bottom: #7B7B7B 4px solid;
                color: #7B7B7B;
                margin-bottom: 3rem;
            }
    }
  @media only screen and (max-width: 426px) and (min-width: 321px){ 
            .lineax{
        border-left:solid 4px #7B7B7B;
        z-index: 0;
        margin-top: 2.5rem;
        width: 0.1rem!important;
        height: auto;
        left: 22.5%;
         min-height: 25rem;
    }
    .ccc{
        max-width: 84%;
        margin: 0 auto!important;
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
        .camnino{
        font-size: 2rem;
        padding: 0;
        border-bottom: #7B7B7B 4px solid;
        color: #7B7B7B;
        margin-bottom: 3rem;
    }
    .izquierda{
        flex: 0 0 41.666667%;
        max-width: 41.666667%;
    }
    .derecha{
        flex: 0 0 41.666667%;
        max-width: 41.666667%;
    }
     .colorDinamicoU{
                background: #ffffff
            }
            .colorDinamicoD{
                background: #DD3B00
            }
            .colorDinamicoT{
                background: #3755E0
            }
               .circle{
                width: 5rem;
                height: 5rem;
                border-radius:100%;
                border:solid 4px  #7B7B7B;
                background-color: #fff;
                position: relative;
            }
                .color-camino{
                color: #7B7B7B;
                margin: 0;
                font-weight: bold;
                text-align: center;
            }
             .camnino{
        font-size: 2rem;
        padding: 0;
        border-bottom: #7B7B7B 4px solid;
        color: #7B7B7B;
        margin-bottom: 3rem;
    }
  }

  @media only screen and (max-width: 600px) and (min-width: 425px) {
         .izquierda{
            flex: 0 0 41.666667%;
            max-width: 41.666667%;
        }
        .derecha{
            flex: 0 0 41.666667%;
            max-width: 41.666667%;
        }
            .lineax{
                border-left:solid 4px #7B7B7B;
                z-index: 0;
                margin-top: 2.5rem;
                width: 0.1rem!important;
                height: auto;
                left: 22%;
                min-height: 25rem;
            }
    .ccc{
        max-width: 84%;
        margin: 0 auto!important;
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
            .colorDinamicoU{
                background: #ffffff
            }
            .colorDinamicoD{
                background: #DD3B00
            }
            .colorDinamicoT{
                background: #3755E0
            }
               .circle{
                width: 5rem;
                height: 5rem;
                border-radius:100%;
                border:solid 4px  #7B7B7B;
                background-color: #fff;
                position: relative;
            }
                .color-camino{
                color: #7B7B7B;
                margin: 0;
                font-weight: bold;
                text-align: center;
            }
             .camnino{
        font-size: 2rem;
        padding: 0;
        border-bottom: #7B7B7B 4px solid;
        color: #7B7B7B;
        margin-bottom: 3rem;
    }
  }
    @media only screen and (max-width: 320px){}
    @media only screen and (max-width: 450px) and (min-width: 321px){}
    @media only screen and (max-width: 600px) and (min-width: 451px) {}
    @media only screen and (max-width: 768px) and (min-width: 601px){
        .lineax{
            border-left:solid 4px #7B7B7B;
            z-index: 0;
            margin-top: 2.5rem;
            width: 100%!important;
            height: 0.1rem;
        }
        .circle {
            width: 4rem;
            height: 4rem;
        }
        .marginsito{
            margin-top: 0.5rem!important;
        }
        .color-camino {
            margin: 0;
            font-weight: bold;
            text-align: center;
            font-size: 0.7rem;
        }
        .camnino {
            font-size: 2rem;
            margin-bottom: 2rem;
        }
    }
    @media only screen and (max-width: 1204px) and (min-width: 769px) {}
</style>