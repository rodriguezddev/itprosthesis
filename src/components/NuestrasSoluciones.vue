<template>
    <div class="cont-nuestras-soluciones">
     
        <div class="ov-hid">
            <h2 class="mejor col-md-5">¿LO MEJOR?</h2>
            <div>
                <div data-aos="fade-right"  class="row trazo-azul m-0 cont-viñeta viñeta-uno clipVi mt-4 mb-4">
                    <div class="alinear">
                        <div class="pl-4 pr-4 mover">
                            <p class="texto-de-azul pl-3">Disfruta de tu nueva prótesis y nuestro programa de empoderamiento desde el primer día a través de una garantía y un pago único mensual.</p>
                        </div>
                        <div data-aos="fade-right" class="tam-paga">
                            <p class="paar text-center">PAGA MENSUALMENTE</p>
                        </div>
                    </div>
                </div>


                 <div data-aos="fade-left"  class="row trazo-rojo  m-0 cont-viñeta viñeta-dos clipViD mt-4 mb-4">
                     <div class="alinearD">
                        <div data-aos="fade-right" class="tam-paga">
                            <p class="paarD text-end">RENOVAMOS TU PRÓTESIS</p>
                        </div>
                        <div class=" pl-4 pr-4  mover">
                            <p class="texto-de-azul protext pl-3">Nunca más te vuelvas a preocupar por comprar una prótesis nueva. En (it) renovamos tu prótesis cada 3 años completamente gratis, nunca más te preocuparás por gastos adicionales.</p>
                        </div>
                     </div>
                </div>


                  <div data-aos="fade-right"  class="row trazo-azul m-0 cont-viñeta viñeta-uno clipVi mt-4 mb-4">
                    <div class="alinear">
                        <div class="pl-4 pr-4  mover">
                            <p class="texto-de-azul pl-3 protext"> Te acompañamos en todo el proceso. Nosotros hacemos el trámite por ti solo preocúpate de escoger la ortopedia de tu preferencia y asistir a las sesiones de nuestro programa.</p>
                        </div>
                        <div data-aos="fade-right" class="tam-paga">
                            <p class="paar cont-ultimo text-center ">DE PRINCIPIO A FIN CONTIGO</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name:'NuestrasSoluciones'
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
        width: 22rem;
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
        clip-path: polygon(0% 0%, 75% 0%, 79% 51%, 75% 100%, 0% 100%);
        width: 365rem;
        transform:translate(-55%)!important;
    }
    .clipViD{
        clip-path: polygon(25% 0%, 100% 0%, 100% 100%, 25% 100%, 18% 47%);
        width: 215rem;
        transform:translate(0%)!important;
    }

    .clipVi:hover{
        transform:translate(0%)!important;
    }
    .clipViD:hover{
        transform: translate(-55.8%)!important;
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
        margin-right: 27rem;
        margin-top: 3rem;
    }
    .paarD{
        font-size: 2rem;
        margin-left: 32rem;
        margin-top: 3rem;
    }
    .protext{
        width: 85rem;
    }
    .cont-ultimo{
        width: 37rem;
        margin-right: 18rem;
    }
    @media only screen and (max-width: 450px){
           .texto-de-azul{
                font-size: 1rem;
                border-left: 2px solid #fff;
            }
            .clipVi {
                -webkit-clip-path: polygon(0% 0%, 75% 0%, 79% 51%, 75% 100%, 0% 100%);
                clip-path: polygon(0% 0%, 75% 0%, 79% 51%, 75% 100%, 0% 100%);
                width: 197rem;
                transform: translate(-66%)!important;
            }
            .clipViD {
                -webkit-clip-path: polygon(25% 0%, 100% 0%, 100% 100%, 25% 100%, 18% 47%);
                clip-path: polygon(25% 0%, 100% 0%, 100% 100%, 25% 100%, 18% 47%);
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
                margin-left: 13rem;
                margin-top: 3rem;
            }
            .mover {
                width: 23rem;
                margin: 0;
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
                margin-right: -2rem;
                margin-top: 3rem;
            }
    }
@media only screen and (max-width: 600px) and (min-width: 451px) { 
    .texto-de-azul{
        font-size: 1rem;
        border-left: 2px solid #fff;
    }
    .clipVi {
        -webkit-clip-path: polygon(0% 0%, 75% 0%, 79% 51%, 75% 100%, 0% 100%);
        clip-path: polygon(0% 0%, 75% 0%, 79% 51%, 75% 100%, 0% 100%);
        width: 197rem;
        transform: translate(-66%)!important;
    }
    .clipViD {
        -webkit-clip-path: polygon(25% 0%, 100% 0%, 100% 100%, 25% 100%, 18% 47%);
        clip-path: polygon(25% 0%, 100% 0%, 100% 100%, 25% 100%, 18% 47%);
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
}
@media only screen and (max-width: 768px) and (min-width: 601px){
  .clipVi{
        clip-path: polygon(0% 0%, 75% 0%, 79% 51%, 75% 100%, 0% 100%);
        width: 196rem!important;
        transform:translate(-55%)!important;
    }
    .texto-de-azul {
        font-size: 1.5rem;
        border-left: 2px solid #fff;
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
        margin-top: 3rem;
    }
    .paarD {
        font-size: 2.5rem;
        margin-left: 25rem;
        margin-top: 3rem;
    }
    .mover {
        width: 50rem!important;
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
}
@media only screen and (max-width: 1204px) and (min-width: 769px) {
     .clipVi{
        clip-path: polygon(0% 0%, 75% 0%, 79% 51%, 75% 100%, 0% 100%);
        width: 245rem;
        transform:translate(-55%)!important;
    }
    .texto-de-azul {
        font-size: 1.5rem;
        border-left: 2px solid #fff;
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
        margin-top: 3rem;
    }
    .mover {
        width: 55rem;
    }
    .clipViD {
        -webkit-clip-path: polygon(25% 0%, 100% 0%, 100% 100%, 25% 100%, 18% 47%);
        clip-path: polygon(25% 0%, 100% 0%, 100% 100%, 25% 100%, 18% 47%);
        width: 157rem;
        transform: translate(-17%)!important;
    }
    .protext {
        width: 56rem;
    }
    .clipViD:hover{
        transform: translate(-57.8%)!important;
    }
    .cont-ultimo{
        width: 40rem;
        margin-right: -3rem;
    }
}
</style>