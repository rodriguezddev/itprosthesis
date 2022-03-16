<template>
    <div class="cont-negro">
         <div class="row justify-content-around max-perfil-tres mb-0 d-none d-md-none d-lg-flex">
            <div class="row flex-column align-items-center m-0 tam-per col-md-4">
                <img src="@/assets/fotosdeperfil/youseph.jpg" alt="" class="perfil-tercera-fila adiez">
                <div class="text-center mt-3">
                    <h5 style=" font-family: 'aileron-bold';" class="cargo-negro">Youseph Yazdi, Ph.D.</h5>
                    <p style=" font-family: 'aileron-bold';" class="cargo">ASESOR EN BIODISEÑO</p>
                </div>
            </div>
            <div class="row flex-column align-items-center m-0 tam-per col-md-4">
                <img src="@/assets/fotosdeperfil/Jose.png" alt="" class="perfil-tercera-fila aonce">
                <div class="text-center mt-3">
                    <h5 style=" font-family: 'aileron-bold';" class="cargo-negro">Jose Gómez</h5>
                    <p style=" font-family: 'aileron-bold';" class="cargo">I&D</p>
                </div>
            </div>
              <div class="row flex-column align-items-center m-0 tam-per col-md-4">
                <img src="@/assets/fotosdeperfil/Wangdo.png" alt="" class="perfil-tercera-fila adoce">
                <div class="text-center mt-3">
                    <h5 style=" font-family: 'aileron-bold';" class="cargo-negro">Wangdo Kim, Ph.D.</h5>
                    <p style=" font-family: 'aileron-bold';" class="cargo">ASESOR GENERAL</p>
                </div>
            </div>
        </div>
        <div class="d-block d-md-block d-lg-none">
              <carousel  :responsive="{0:{items:1,nav:false},600:{items:3,nav:true}}">
                <div>
                    <div class="row flex-column align-items-center m-0 tam-per">
                        <img src="@/assets/fotosdeperfil/Wangdo.png" alt="" class="perfil-tercera-fila adoce">
                        <div class="text-center mt-3">
                            <h5 style=" font-family: 'aileron-bold';" class="cargo-negro">Wangdo Kim, Ph.D.</h5>
                            <p style=" font-family: 'aileron-bold';" class="cargo">ASESOR GENERAL</p>
                        </div>
                    </div>
                </div>
                <div>
                    <div class="row flex-column align-items-center m-0 tam-per">
                        <img src="@/assets/fotosdeperfil/Jose.png" alt="" class="perfil-tercera-fila aonce">
                        <div class="text-center mt-3">
                            <h5 style=" font-family: 'aileron-bold';" class="cargo-negro">Jose Gómez</h5>
                            <p style=" font-family: 'aileron-bold';" class="cargo">I&D</p>
                        </div>
                    </div>
                </div>
                <div>
                      <div class="row flex-column align-items-center m-0 tam-per">
                        <img src="@/assets/fotosdeperfil/youseph.jpg" alt="" class="perfil-tercera-fila adiez">
                        <div class="text-center mt-3">
                            <h5 style=" font-family: 'aileron-bold';" class="cargo-negro">Youseph Yazdi, Ph.D.</h5>
                            <p style=" font-family: 'aileron-bold';" class="cargo">ASESOR EN BIODISEÑO</p>
                        </div>
                    </div>
                </div>
              </carousel>
        </div>
    </div>
</template>
<script>
import carousel from 'vue-owl-carousel'
export default {
    name:'CargosNegro',
    components: { 
        carousel 
    },
    data() {
      return {
        swiperOption: {
          slidesPerView: 4,
          spaceBetween: 30,
          centeredSlides: true,
          pagination: {
            el: '.swiper-pagination',
            clickable: true
          }
        },
      }
    }
}
</script>
<style>
    .cont-negro{
        background: black;
        width: 100%;
        padding: 4rem 2rem;
    }
    .cargo-negro{
        color:#fff
    }
    .adiez{
        border: solid 5px #7B635E;
        border-radius: 100%;
    }
    .aonce{
        border: solid 5px #4A7C43;
        border-radius: 100%;
    }
     .adoce{
        border: solid 5px #7B635E;
        border-radius: 100%;
    }
</style>