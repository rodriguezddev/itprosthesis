<template>
    <div data-aos="zoom-out" class="margin-equipo" :style="'background:' + fondo" style="transition: 0.4s all ease;">
        <div class="row justify-content-end m-0">
            <h2 class="Equipo col-md-3">EQUIPO</h2>
        </div>
        <div  class="row justify-content-around max-perfil">
            <div class="row flex-column align-items-center m-0 tam-per" @mouseover="agg(ids[0])" @mouseout="volver()">
                <img src="@/assets/fotosdeperfil/Piero.jpg" alt="" class="perfil-primera-fila auno">
                <div class="text-center">
                    <h4>Piero comsme</h4>
                    <h5 class="cargo" :class="{cargoHo : sobre}" >FUNDADOR Y CEO</h5>
                    <a href="#" class="colorsTO">Linkedin</a>
                </div>
            </div>
            <div class="row flex-column align-items-center m-0 tam-per" @mouseover="agg(ids[1])" @mouseout="volver()">
                <img src="@/assets/fotosdeperfil/Franco.jpg" alt="" class="perfil-primera-fila ados">
                <div class="text-center">
                    <h4>Franco Carlini</h4>
                    <h5 class="cargo" :class="{cargoHo : sobre}">FUNDADOR Y COO</h5>
                    <a href="#" class="colorsTO">Linkedin</a>
                </div>
            </div>
        </div>

         <div  class="row justify-content-around max-perfil-dos">
            <div class="row flex-column align-items-center m-0 tam-per" @mouseover="agg(ids[2])" @mouseout="volver()">
                <img src="@/assets/fotosdeperfil/dunia.jpg" alt="" class="perfil-segunda-fila atres">
                <div class="text-center">
                    <h4>Dunia Felices</h4>
                    <h5 class="cargo" :class="{cargoHo : sobre}">CCO</h5>
                    <a href="#" class="colorsTO">Linkedin</a>
                </div>
            </div>
            <div class="row flex-column align-items-center m-0 tam-per" @mouseover="agg(ids[3])" @mouseout="volver()">
                <img src="@/assets/fotosdeperfil/Renato.jpg" alt="" class="perfil-segunda-fila acuatro">
                <div class="text-center">
                    <h4>Renato Corahua</h4>
                    <h5 class="cargo" :class="{cargoHo : sobre}">LIDER DE I&D</h5>
                    <a href="#" class="colorsTO">Linkedin</a>
                </div>
            </div>
              <div class="row flex-column align-items-center m-0 tam-per" @mouseover="agg(ids[4])" @mouseout="volver()">
                <img src="@/assets/fotosdeperfil/Mariana.jpg" alt="" class="perfil-segunda-fila acinco">
                <div class="text-center">
                    <h4>Mariana De La Piedra</h4>
                    <h5 class="cargo" :class="{cargoHo : sobre}">LIDER DE IMPACTO SOCIAL</h5>
                    <a href="#" class="colorsTO">Linkedin</a>
                </div>
            </div>
        </div>

         <div class="row justify-content-around max-perfil-tres">
            <div class="row flex-column align-items-center m-0 tam-per" @mouseover="agg(ids[5])" @mouseout="volver()">
                <img src="@/assets/fotosdeperfil/Steve.jpg" alt="" class="perfil-tercera-fila aseis">
                <div class="text-center">
                    <h4>Steve Surichanqui</h4>
                    <h5 class="cargo" :class="{cargoHo : sobre}">I&D</h5>
                    <a href="#" class="colorsTO">Linkedin</a>
                </div>
            </div>
            <div class="row flex-column align-items-center m-0 tam-per" @mouseover="agg(ids[6])" @mouseout="volver()">
                <img src="@/assets/fotosdeperfil/Luz.jpg" alt="" class="perfil-tercera-fila asiete">
                <div class="text-center">
                    <h4>Luz Melgarejo</h4>
                    <h5 class="cargo" :class="{cargoHo : sobre}">IMPACTO SOCIAL</h5>
                    <a href="#" class="colorsTO">Linkedin</a>
                </div>
            </div>
              <div class="row flex-column align-items-center m-0 tam-per" @mouseover="agg(ids[7])" @mouseout="volver()">
                <img src="@/assets/fotosdeperfil/Piero.jpg" alt="" class="perfil-tercera-fila aocho">
                <div class="text-center">
                    <h4>Daniella Rivero</h4>
                    <h5 class="cargo" :class="{cargoHo : sobre}">I&D</h5>
                    <a href="#" class="colorsTO">Linkedin</a>
                </div>
            </div>
              <div class="row flex-column align-items-center m-0 tam-per" @mouseover="agg(ids[8])" @mouseout="volver()">
                <img src="@/assets/fotosdeperfil/Aaron.jpg" alt="" class="perfil-tercera-fila anueve">
                <div class="text-center">
                    <h4>Aaron Llican</h4>
                    <h5 class="cargo" :class="{cargoHo : sobre}">I&D</h5>
                    <a href="#" class="colorsTO">Linkedin</a>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name:'Equipo',
    data() {
        return {
            colores:[
                '#D57521', '#89D841', '#D70000', '#cfc17c;', '#852DDD', '#6275E6', '#CC8A81','#C89700', '#6CBDE4'
            ],
            ids:[0, 1, 2, 3, 4, 5, 6, 7, 8],
            fondo:'#ffffff',
            sobre:false
        }
    },
    methods:{
        agg(index){
            this.fondo = this.colores[index],
            this.sobre = true
        },
        volver(){
            this.fondo = '#ffffff'
            this.sobre = false
        }
    }
}
</script>
<style>
    .auno{
        border: solid 5px #D57521;
        border-radius: 100%;
    }
    .ados{
        border: solid 5px #89D841;
        border-radius: 100%;
    }
    .atres{
        border: solid 5px #D70000;
        border-radius: 100%;
    }
    .acuatro{
        border: solid 5px #cfc17c;
        border-radius: 100%;
    }
    .acinco{
        border: solid 5px #852DDD;
        border-radius: 100%;
    }
    .aseis{
        border: solid 5px #6275E6;
        border-radius: 100%;
    }
    .asiete{
        border: solid 5px #CC8A81;
        border-radius: 100%;
    }
    .aocho{
        border: solid 5px #C89700;
        border-radius: 100%;
    }
    .anueve{
        border: solid 5px #6CBDE4;
        border-radius: 100%;
    }
     .Equipo{
        margin-left:3rem;
        font-size: 2.8rem;
        padding: 0;
        margin-bottom:4rem;
    }
    .Equipo::after{
        content: '';
        display: block;
        height: 0.2rem;
        width: 100%;
        background-color: rgb(63, 63, 63);
    }
    .margin-equipo{
        margin-top: 5rem; 
        transition: 0.4s all ease;
    }
    .perfil-primera-fila{
        border-radius: 100%;
        width: 23rem;
        height: 23rem;
    }
    .perfil-segunda-fila{
        border-radius: 100%;
        width: 23rem;
        height: 23rem;
    }
    .perfil-tercera-fila{
        border-radius: 100%;
        width: 17rem;
        height: 17rem;
    }
    .cargo{
        color:rgb(169, 172, 173)
    }
    .cargoHo{
        color:#fff!important;
    }
    .max-perfil{
        max-width: 75rem;
        margin: 0rem auto 0rem auto!important;
        padding-bottom: 5rem;
    }
     .max-perfil-dos{
        max-width: 85rem;
        margin: 0rem auto 0rem auto!important;
        padding-bottom: 5rem;
       
    }
     .max-perfil-tres{
        max-width: 95rem;
        margin: 0rem auto 0rem auto!important;
        padding-bottom: 5rem;
    }
    .colorsTO{
        color: black;
    }
    .colorsTO:hover{
        color: black;
        text-decoration: none;
    }
    @media only screen and (max-width: 600px){ 
    .perfil-primera-fila {
        border-radius: 100%;
        width: 10rem;
        height: 10rem;
    }
    .perfil-segunda-fila {
        border-radius: 100%;
        width: 10rem;
        height: 10rem;
    }
     .perfil-tercera-fila {
        border-radius: 100%;
        width: 10rem;
        height: 10rem;
    }
}
@media only screen and (max-width: 768px) {
    .color-contacto{
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        height: 20rem;
    }
}
</style>