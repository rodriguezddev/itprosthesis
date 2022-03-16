<template>
    <div class="cont-nuestras-soluciones" >
     
        <div class="ov-hid">
            <h2 class="nuestros col-md-4 col-8 text-right p-0" style=" font-family: 'Kollektif';">¿LO MEJOR?</h2>

            <div class="d-block d-md-block d-lg-block" @mouseout="volver()">
                <div class="d-flex contenedor-viñeta-mobile">
                    <div  class="row trazo-azul m-0  transision-de-width" @mouseover="agUD(id[0])"  :class="[showA == 1 ? 'item-viñeta-mobile' : showA == 2 ? 'agrandar' : showA == 3 ? 'otras' : '' ]" >
                        <div class="con-texto-viñeta" :class="[texto ? 'max-abierto' : '' ]">
                            <div  class=" h-100 row m-0 align-items-center">
                                <p class="tam-titu" style=" font-family: 'Kollektif';" :class="[ showA == 3 ? 'titulito' : '' ]">PAGA MENSUALMENTE</p>
                                <p class="texto-de-azul pl-3 text3__text  " :class="[texto ? 'text3__abierto' :  '' ]">Disfruta de tu nueva prótesis y nuestro programa de empoderamiento desde el primer día a través de una garantía y un pago único mensual.</p>
                            </div>
                        </div>
                    </div>

                    <div  class="row trazo-rojo  m-0   item-viñeta-mobile transision-de-width" @mouseover="agDD(id[1])" :class="[showB == 1 ? 'item-viñeta-mobile' : showB == 2 ? 'agrandar' : showB == 3 ? 'otras' : '' ]">
                        <div class="con-texto-viñeta" :class="[textoD ? 'max-abierto' : '' ]">
                            <div class=" h-100 row m-0 align-items-center">
                                <p class="tam-titu" style=" font-family: 'Kollektif';" :class="[ showB == 3 ? 'titulito' : '' ]">RENOVAMOS<br/> TU PRÓTESIS</p>
                            
                                <p class="texto-de-azul t-dos pl-3 text3__text " :class="[textoD ? 'text3__abierto' : '' ]">Nunca más te vuelvas a preocupar por comprar una prótesis nueva. En (it) renovamos tu prótesis cada 3 años completamente gratis, nunca más te preocuparás por gastos adicionales.</p>
                            </div>
                        </div>
                    </div>

                    <div  class="row trazo-azul m-0  item-viñeta-mobile transision-de-width" @mouseover="agTD(id[2])"  :class="[showC == 1 ? 'item-viñeta-mobile' : showC == 2 ? 'agrandar' : showC == 3 ? 'otras' : '' ]">
                        <div class="con-texto-viñeta" :class="[textoT ? 'max-abierto' : '' ]">
                            <div class="  h-100 row m-0 align-items-center">
                                <p class="tam-titu" style=" font-family: 'Kollektif';" :class="[ showC == 3 ? 'titulito' : '' ]">DE PRINCIPIO<br/> A FIN CONTIGO</p>
                      
                                <p class="texto-de-azul pl-3 t-uno text3__text " :class="[textoT ? 'text3__abierto' : '' ]"> Te acompañamos en todo el proceso. Nosotros hacemos el trámite por ti solo preocúpate de escoger la ortopedia de tu preferencia y asistir a las sesiones de nuestro programa.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name:'NuestrasSoluciones',
    data(){
        return{
            id:[0,1,2],
            showA:1,
            showB:1,
            showC:1,
            texto:false,
            textoD:false,
            textoT:false
        }
    },
    methods:{
        agUD(){
            this.showA = 2
            var that = this
            that.texto = true
            if (this.showA == 2) {
                setTimeout(function(){ 
                    
                }, 300);
            }
            this.showC = 3
            this.showB = 3
            this.textoD = false
            this.textoT = false
            console.log(this.showB,this.showA, this.texto , this.textoD ,  this.showC,  this.textoT )
        },
        agDD(){
            this.showB = 2
             var that = this
              that.textoD = true
             this.showC = 3
             this.showA = 3
             this.texto = false
             this.textoT = false
             console.log(this.showB,this.showA, this.texto , this.textoD ,  this.showC,  this.textoT )
        },
        agTD(){
            this.showC = 2
             var that = this
              that.textoT = true
            
            this.showB = 3
            this.showA = 3
            this.texto = false
            this.textoD = false
            console.log(this.showB,this.showA, this.texto , this.textoD ,  this.showC,  this.textoT )
        },
        volver(){
             this.showC = 1
             this.showB = 1
             this.showA = 1
             this.texto = false
             this.textoD = false
             this.textoT = false
             console.log( this.showC, this.showB,  this.showA, this.texto,  this.textoD,  this.textoT )
        }

    }
}
</script>
<style>
    .cont-nuestras-soluciones{
        margin-top: 5rem;
    }
     .mejor{
        margin-left:3rem;
        font-size: 2.8rem;
        padding: 0;
        margin-bottom:2rem;
    }
    .mejor::after{
        content: '';
        display: block;
        height: 0.2rem;
        width: 20rem;
        background-color:   rgb(63, 63, 63);
        margin-left:-3.6rem;
    }
    .trazo-azul{
        color:#fff;
        background-color:#3755E0;
        padding: 2rem 0rem;
        
    }
    .texto-de-azul{
        font-size: 1.5rem;
        border-left: 2px solid #fff;
    }
    .viñeta-estilo{
        font-weight: bold
    }
    .ov-hid{
        overflow: hidden;
        margin: 2rem 0rem
    }
    .trazo-rojo{
        background: #DD3B00;
        color:#fff;
        padding: 2rem 0rem;
        margin: 2rem 0rem;
    }
    .clipVi{
        clip-path: polygon(0% 0%, 76% 0%, 79% 51%, 76% 100%, 0% 100%);
        width: 365rem;
        transform: translate(-65%)!important;
    }
    .clipViD{
        clip-path: polygon(20% 0%, 100% 0%, 100% 100%, 20% 100%, 18% 47%);
        width: 365rem;
        transform: translate(-8%)!important;
    }

    .clipVi:hover{
        transform:translate(0%)!important;
    }
    .clipViD:hover{
        transform: translate(-61%)!important;
    }
    .mover{
        width: 75rem;
        font-size: 0.9rem
    }
    .tam-paga{
        width: 75rem;
        display: contents;
    }
    .alinear{
        width: 71%;
        display: flex;
        justify-content: space-between;
    }
    .alinearD{
        width: 100%;
        display: flex;
        justify-content: space-around;
    }
    .paar{
        font-size: 2rem;
        margin-right: -8rem;
        margin-top: 1rem;
    }
    .paarD{
        font-size: 2rem;
        margin-left: 10rem;
        margin-top: 2rem;
    }
    .protext{
        width: 85rem;
    }
    .cont-ultimo{
        width: 37rem;
        margin-right: -24rem;
    }
    .item-viñeta-mobile{
        width: 33.33%
    }
    .agrandar{
        transition: width 0.3s ease;
        width:80%
    }
    .otras{
        transition: width 0.3s ease;
        width:10%!important;
        
    }
    .titulito{
        transition: opacity 0.3s ease-out;
        opacity: 0;
    }

    .tam-titu{
        width: 15rem;
        font-size: 1.9rem
    }
    .text3__text {
        height: 0;
        opacity: 0;
        transform: translateY(-10%);
        transition: opacity 0.3s ease-out, transform 0.3s ease-out;
        font-size:1.2rem
    }
    .text3__abierto {
        height: auto;
        opacity: 1;
        transform: translateY(0);
        transition: opacity 0.3s ease-out, transform 0.3s ease-out;
    }
    
    
    .transision-de-width{
        transition: width 0.5s ease-out;
    }
    .contenedor-viñeta-mobile{
        height: 20rem;
    }
    .con-texto-viñeta{
        padding: 2rem
    }
    .max-abierto{
        max-width: 60rem;
        margin: 0 auto;
    }
    @media only screen and (max-width: 450px){
           .texto-de-azul{
                font-size: 0.8rem;
                border-left: 2px solid #fff;
                margin: 0.5rem;
            }
            .clipVi {
                width: 197rem;
                transform: translate(-66%)!important;
            }
            .clipViD {
                width: 141rem;
                transform: translate(-18%)!important;
            }
            .alinear {
                width: 90%;
                display: flex;
                justify-content: space-between;
            }
            .paar {
                font-size: 1.1rem;
                margin-right: 31rem;
                margin-top: 2rem;
            }
            .paarD {
                font-size: 1.5rem;
                margin-left: 13rem;
                margin-top: 3rem;
            }
            .mover {
                width: 20rem;
                margin: 0
            }
            .protext {
                width: 21rem;
                margin: 0;
            }
            .alinearD {
                width: 83%;
                display: flex;
                justify-content: space-around;
            }
            .cont-ultimo {
                width: 75rem;
                margin-right: -32rem!important;
                margin-top: 0.5rem;
                margin-bottom: 0.5rem;
            }
            .trazo-azul {
                color: #fff;
                background-color: #3755E0;
                padding: 0rem; 
            }
            .trazo-rojo {
                background: #DD3B00;
                color: #fff;
                padding: 0rem;
                margin: 2rem 0rem;
            }
            .texto-paciente {
                font-size: 4rem;
                font-family: 'Roboto';
            }
            .borde-paciene-uno {
                border-right: solid 0.5rem #DD3B00;
                margin-left: 0rem;
            }
            .borde-paciene-dos {
                border-left: solid 0.5rem #2359E5;
                margin-right: 4rem;
            }
            .borde-paciene-tres {
                border-right: solid 0.5rem #F7E200;
                margin-left: 3rem;
            }
            .borde-paciene-cuatro {
                border-left: solid 1.3rem #66B42B;
                margin-right: 2rem;
            }
            .paciente {
                width: 13rem;
                margin-top: 2rem;
            }
            .item-paciente {
                font-size: 1.5rem;
                font-family: 'Roboto';
            }
         .tam-titu {
            width: 8rem;
            font-size: 0.8rem;
        }
        .con-texto-viñeta {
            padding: 1rem;
        }
        .contenedor-viñeta-mobile {
            height: 13rem;
        }
    }
@media only screen and (max-width: 600px) and (min-width: 451px) { 
    .texto-de-azul{
        font-size: 1rem;
        border-left: 2px solid #fff;
    }
    .clipVi {
        width: 197rem;
        transform: translate(-66%)!important;
    }
    .clipViD {
        width: 141rem;
        transform: translate(-18%)!important;
    }
    .alinear {
        width: 90%;
        display: flex;
        justify-content: space-between;
    }
    .paar {
        font-size: 1.5rem;
        margin-right: 29rem;
        margin-top: 2rem;
    }
    .paarD {
        font-size: 1.5rem;
        margin-left: 16rem;
        margin-top: 3rem;
    }
    .mover {
        width: 29rem;
        margin: 0;
    }
    .protext {
        width: 23rem;
        margin: 0;
    }
    .alinearD {
        width: 87%;
        display: flex;
        justify-content: space-around;
    }
    .cont-ultimo {
        width: 75rem;
        margin-right: -2rem;
        margin-top: 3rem;
    }
    .tam-titu {
        width: 11rem;
        font-size: 1.5rem;
    }
        .contenedor-viñeta-mobile {
            height: 15rem;
        }
}
@media only screen and (max-width: 768px) and (min-width: 601px){
  .clipVi{
        width: 196rem!important;
        transform:translate(-55%)!important;
  }
      .texto-de-azul {
        font-size: 1.5rem;
        border-left: 2px solid #fff;
    }
    .trazo-azul {
        color: #fff;
        background-color: #3755E0;
        padding: 1rem 0rem;
    }
    .trazo-rojo{
        background: #DD3B00;
        color:#fff;
        padding: 1rem 0rem;
    }
    .linea {
        border-left: solid 4px #fff;
        z-index: 0;
        margin-top: 0.5rem;
        left: 50%;
        width: 0.1px;
        height: 100%;
    }
     .paar{
        font-size: 2rem;
        margin-right: 7rem;
        margin-top: 1rem;
    }
     .paarD{
        font-size: 2rem;
        margin-left: 32rem;
        margin-top: 1rem;
    }
    .cont-ultimo {
        width: 40rem;
        margin-right: -11rem!important;
    }
    .clipViD {
        -webkit-clip-path: polygon(25% 0%, 100% 0%, 100% 100%, 25% 100%, 18% 47%);
        clip-path: polygon(25% 0%, 100% 0%, 100% 100%, 25% 100%, 18% 47%);
        width: 157rem;
        transform: translate(-17%)!important;
    }
    .protext {
        width: 46rem;
    }
    .clipViD:hover{
        transform: translate(-60.8%)!important
    }
    .alinear {
        width: 74%;
        display: flex;
        justify-content: space-between;
    }
    .cont-ultimo {
        width: 40rem;
        margin-right: -2rem;
    }
    .tam-titu {
        width: 15rem;
        font-size: 1.7rem;
    }
    .texto-de-azul {
        font-size: 1rem;
        border-left: 2px solid #fff;
    }
           .contenedor-viñeta-mobile {
            height: 17rem;
        }
}
@media only screen and (max-width: 1204px) and (min-width: 769px) {
     .clipVi{
        width: 245rem;
        transform:translate(-55%)!important;
    }
    .texto-de-azul {
        font-size: 1.5rem;
        border-left: 2px solid #fff;
    }
    .trazo-azul {
        color: #fff;
        background-color: #3755E0;
        padding: 1rem 0rem;
    }
    .trazo-rojo{
        background: #DD3B00;
        color:#fff;
        padding: 1rem 0rem;
    }
    .linea {
        border-left: solid 4px #fff;
        z-index: 0;
        margin-top: 0.5rem;
        left: 50%;
        width: 0.1px;
        height: 100%;
    }
     .paar{
        font-size: 2.5rem;
        margin-right: 7rem;
        margin-top: 1rem;
    }
     .paarD{
        font-size: 2rem;
        margin-left: 32rem;
        margin-top: 1rem;
    }
    .mover {
        width: 55rem;
    }
    .clipViD {
        width: 173rem;
        transform: translate(-17%)!important;
    }
    .protext {
        width: 56rem;
    }
    .clipViD:hover{
        transform: translate(-57.8%)!important;
    }
}
@media only screen and (max-width: 1440px) and (min-width: 1205px){
      .clipViD{
        width: 365rem;
        transform: translate(-8%)!important;
    }
    .clipViD:hover {
        transform: translate(-62.7%)!important;
    }
    .clipVi:hover {
        transform: translate(0%)!important;
    }
    .mover{
        margin-left: 3rem;
    }

}
@media only screen and (max-width: 1881px) and (min-width: 1441px){
       .clipViD{
        width: 365rem;
        transform: translate(-1%)!important;
    }
    .clipVi{
            width: 196rem!important;
            transform: translate(-63%)!important;
    }
}
@media only screen and (max-width: 2560px) and (min-width: 1880px){
       .clipViD{
        width: 365rem;
        transform: translate(0%)!important;
    }
}
@media only screen and (min-width: 2561px){
       .clipViD{
        width: 365rem;
        transform: translate(0%)!important;
    }
}
</style>