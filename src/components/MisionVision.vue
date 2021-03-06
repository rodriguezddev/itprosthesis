<template>
<div>
    <div class="contMisionVision row mr-0 ml-0 d-xl-flex d-lg-flex d-md-none d-none">
        <div data-aos="fade-right" class="mision contorno col-md-8">
            <div class=" col-md-6">
                <p class="textoMV">Proveer de soluciones integrales en materia de tecnologia y  formación a toda la población latinoamericana de personas con una amputación de miembro inferior a través de un  modelo de negocio coherente y accesible para ellos</p>
                <h4 class="titleMV">MISIÓN</h4>
            </div>
        </div>
        <div data-aos="fade-left" class="vision contorno col-md-9 row flex-column align-items-end m-0">
            <div class="col-md-6 text-right">
                <h4 class="titleMV">VISIÓN</h4>
                <p class="textoMV">Eliminar las brechas sociales de la persona con discapacida física en Latinoamérica por medio de nuestros clientes empoderados, los cuales serán capaces de exigir sus derechos con recursos y argumentos válidos</p>
            </div>
        </div>
    </div>

     <div class="contMisionVision row mr-0 ml-0 d-xl-none d-lg-none d-md-flex d-flex">
        <div data-aos="fade-right" class="misionD contorno col-12">
            <div class=" col-12">
                <p class="textoMV">Proveer de soluciones integrales en materia de tecnologia y  formación a toda la población latinoamericana de personas con una amputación de miembro inferior a través de un modelo de negocio coherente y accesible para ellos</p>
                <h4 class="titleMV">MISIÓN</h4>
            </div>
        </div>
        <div data-aos="fade-left" class="visionD contorno col-12 row flex-column align-items-end m-0">
            <div class=" col-12 text-right">
                <h4 class="titleMV">VISIÓN</h4>
                <p class="textoMV">Eliminar las brechas sociales de la persona con discapacidad física en Latinoamérica por medio de nuestros clientes empoderados, los cuales serán capaces de exigir sus derechos con recursos y argumentos válidos</p>
            </div>
        </div>
    </div>
</div>
</template>
<script>
export default {
    name:'MisionVision'
}
</script>
<style>
    .contMisionVision{
        height: 25rem;
        overflow: hidden;
    }
    
    .mision{
        background: #2359E5;
        color:#fff;
        font-family: 'Roboto', sans-serif;
        padding:2rem;
        clip-path: polygon(100% 0, 0 0,0 185%);
        position:absolute!important;
        left:0;
        height: 25rem;
        z-index: 2;
    }
    .vision{
        background: #FF3A12;
        color:#fff;
        font-family: 'Roboto', sans-serif;
        padding:2rem;
        clip-path: polygon(101% 100%, 0% 100%,100% -161%);
        position:absolute!important;
        right:0;
        height: 25rem;
    }

    .textoMV{
        line-height: 2;
        letter-spacing: 2px;
        font-size:1.1rem
    }
    .titleMV{
        font-size: 43px;
    }
@media only screen and (max-width: 600px){ 
     .contMisionVision{
        height: 100%;
        overflow: hidden;
    }
        .misionD{
        background: #2359E5;
        color:#fff;
        font-family: 'Roboto', sans-serif;
        padding:2rem;
        left:0;
        height: 100%;
        z-index: 2;
    }
    .visionD{
        background: #FF3A12;
        color:#fff;
        font-family: 'Roboto', sans-serif;
        padding:2rem;
        right:0;
        height: 100%
    }
}
@media only screen and (max-width: 768px) {
     .contMisionVision{
        height: 100%;
        overflow: hidden;
    }
    .mision{
        height: 30rem;
    }
    .vision{
        height: 30rem;
    }
         .misionD{
        background: #2359E5;
        color:#fff;
        font-family: 'Roboto', sans-serif;
        padding:2rem;
        left:0;
        height: 100%;
        z-index: 2;
    }
    .visionD{
        background: #FF3A12;
        color:#fff;
        font-family: 'Roboto', sans-serif;
        padding:2rem;
        right:0;
        height: 100%
    }
}
@media only screen and (max-width: 995px) {
     .contMisionVision{
        height: 100%;
        overflow: hidden;
    }
    .mision{
        height: 30rem;
    }
    .vision{
        height: 30rem;
    }
         .misionD{
        background: #2359E5;
        color:#fff;
        font-family: 'Roboto', sans-serif;
        padding:2rem;
        left:0;
        height: 100%;
        z-index: 2;
    }
    .visionD{
        background: #FF3A12;
        color:#fff;
        font-family: 'Roboto', sans-serif;
        padding:2rem;
        right:0;
        height: 100%
    }
}
</style>