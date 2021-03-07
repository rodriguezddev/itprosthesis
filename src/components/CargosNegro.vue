<template>
    <div class="cont-negro">
         <div class="row justify-content-around max-perfil-tres mb-0">
            <div class="row flex-column align-items-center m-0 tam-per">
                <img src="@/assets/fotosdeperfil/youseph.jpg" alt="" class="perfil-tercera-fila adiez">
                <div class="text-center mt-3">
                    <h5 class="cargo-negro">Youseph Yazdi</h5>
                    <p class="cargo">ASESOR EN BIODISEÑO</p>
                </div>
            </div>
            <div class="row flex-column align-items-center m-0 tam-per">
                <img src="@/assets/fotosdeperfil/Jose.jpg" alt="" class="perfil-tercera-fila aonce">
                <div class="text-center mt-3">
                    <h5 class="cargo-negro">Jose Gómez</h5>
                    <p class="cargo">I&D</p>
                </div>
            </div>
              <div class="row flex-column align-items-center m-0 tam-per">
                <img src="@/assets/fotosdeperfil/chino.png" alt="" class="perfil-tercera-fila adoce">
                <div class="text-center mt-3">
                    <h5 class="cargo-negro">Wangdo Kim</h5>
                    <p class="cargo">ASESOR GENERAL</p>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name:'CargosNegro'
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