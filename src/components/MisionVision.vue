<template>
<div>
    <div class="contMisionVision row mr-0 ml-0 d-xl-flex d-lg-flex d-md-none d-none">
        <div data-aos="fade-right" data-aos-duration="2000" class="mision contorno">
            <div class="">
                <p class="textoMV">Proveer de soluciones integrales en materia de tecnología y<br/>  formación a toda la población latinoamericana <br/> de personas con una amputación de <br/> miembro inferior a través de un <br/>  modelo de negocio coherente <br/> y accesible para ellos.</p>
                <h4 class="titleMV">MISIÓN</h4>
            </div>
        </div>
        <div data-aos="fade-left" data-aos-duration="2000" class="vision contorno row flex-column align-items-end m-0">
            <div class="text-right col-md-9">
                <h4 class="titleMV">VISIÓN</h4>
                <p class="textoMV">Eliminar las brechas sociales <br/> de la persona con discapacidad<br/> física en Latinoamérica por medio de  <br/>nuestros clientes empoderados, los cuales serán <br/> capaces de exigir sus derechos con recursos y argumentos <br/> válidos.</p>
            </div>
        </div>
    </div>

     <div class="contMisionVision row mr-0 ml-0 d-xl-none d-lg-none d-md-flex d-flex">
        <div data-aos="fade-right" data-aos-duration="2000" class="misionD contorno col-12">
            <div class=" col-12">
                <p class="textoMV duplicado">Proveer de soluciones integrales en materia de tecnología y  formación a toda la población latinoamericana de personas con una amputación de miembro inferior a través de un modelo de negocio coherente y accesible para ellos.</p>
                <h4 class="titleMV ">MISIÓN</h4>
            </div>
        </div>
        <div data-aos="fade-left" data-aos-duration="2000" class="visionD contorno col-12 row flex-column align-items-end m-0">
            <div class=" col-12 text-right">
                <h4 class="titleMV ">VISIÓN</h4>
                <p class="textoMV duplicado">Eliminar las brechas sociales de la persona con discapacidad física en Latinoamérica por medio de nuestros clientes empoderados, los cuales serán capaces de exigir sus derechos con recursos y argumentos válidos.</p>
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
        font-family: 'Kollektif';
        padding:2rem;
        clip-path: polygon(100% 0, 50% 100%, 0 100%, 0 0);
        position:absolute!important;
        left:0;
        height: 21rem;
        z-index: 2;
        width: 67%;
    }
    .vision{
        background: #FF3A12;
        color:#fff;
        font-family: 'Kollektif';
        padding:2rem;
        clip-path: polygon(50% 0, 100% 0, 100% 100%, 0 100%);
        position:absolute!important;
        right:0;
        height: 21rem;
        width: 67%
    }

    .textoMV{
        line-height: 2;
        letter-spacing: 2px;
        font-size:1.1rem;
        font-family: 'Kollektif';
    }
    .titleMV{
        font-size: 43px;
    }
    .duplicado{
        text-align: justify
    }
    .contorno{
        overflow: hidden;
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