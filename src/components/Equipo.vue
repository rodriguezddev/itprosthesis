<template>
    <div data-aos="zoom-out" class="margin-equipo"  style="transition: 0.4s all ease;">
        <div class="row justify-content-end m-0">
            <h2 class="Equipo col-md-3">EQUIPO</h2>
        </div>
        <div  class="row justify-content-cernter max-uno">
            <div class="row flex-column align-items-center m-0 tam-per" @mouseover="agg(ids[0])" :style="'background:' + fondo" @mouseout="volver()">
                <img src="@/assets/fotosdeperfil/Piero.jpg" alt="" class="perfil-primera-fila auno">
                <div class="text-center">
                    <h4>Piero Comsme</h4>
                    <h5 class="cargo" :class="{cargoHo : sobre}" >FUNDADOR Y CEO</h5>
                    <a href="https://www.linkedin.com/in/piero-cosme-velasco-01390b140/" class="colorsTO">Linkedin</a>
                </div>
            </div>
            <div class="row flex-column align-items-center m-0 tam-per" @mouseover="aggi(ids[1])" :style="'background:' + fondoi" @mouseout="volver()">
                <img src="@/assets/fotosdeperfil/Franco.jpg" alt="" class="perfil-primera-fila ados">
                <div class="text-center">
                    <h4>Franco Carlini</h4>
                    <h5 class="cargo" :class="{cargoHo : sobrea}">FUNDADOR Y COO</h5>
                    <a href="https://www.linkedin.com/in/franco-giovanni-carlini-camaiora-912b9a149/" class="colorsTO">Linkedin</a>
                </div>
            </div>
        </div>

         <div  class="row justify-content-around max-dos">
            <div class="row flex-column align-items-center m-0 tam-per-card-s col-lg-4 col-md-4" @mouseover="agga(ids[2])" :style="'background:' + fondoa" @mouseout="volver()">
                <img src="@/assets/fotosdeperfil/dunia.jpg" alt="" class="perfil-segunda-fila atres">
                <div class="text-center">
                    <h4>Dunia Felices</h4>
                    <h5 class="cargo" :class="{cargoHo : sobreb}">CCO</h5>
                    <a href="https://instagram.com/duniafelices?igshid=mjn7cb8zrysk" class="colorsTO">Instagram</a>
                </div>
            </div>
            <div class="row flex-column align-items-center m-0 tam-per-card-s col-lg-4 col-md-4" @mouseover="aggb(ids[3])" :style="'background:' + fondob" @mouseout="volver()">
                <img src="@/assets/fotosdeperfil/Renato.jpg" alt="" class="perfil-segunda-fila acuatro">
                <div class="text-center">
                    <h4>Renato Corahua</h4>
                    <h5 class="cargo" :class="{cargoHo : sobrec}">LIDER DE I&D</h5>
                    <a href="https://www.linkedin.com/in/renato-corahua-benites/" class="colorsTO">Linkedin</a>
                </div>
            </div>
              <div class="row flex-column align-items-center m-0 tam-per-card-s col-lg-4 col-md-4" @mouseover="aggc(ids[4])" :style="'background:' + fondoc" @mouseout="volver()">
                <img src="@/assets/fotosdeperfil/Mariana.jpg" alt="" class="perfil-segunda-fila acinco">
                <div class="text-center">
                    <h4>Mariana De La Piedra</h4>
                    <h5 class="cargo" :class="{cargoHo : sobred}">LIDER DE IMPACTO SOCIAL</h5>
                    <a href="https://www.linkedin.com/in/mariana-de-la-piedra-alayza-907566131/" class="colorsTO">Linkedin</a>
                </div>
            </div>
        </div>

         <div class="row justify-content-around max-perfil-tres">
            <div class="row flex-column align-items-center m-0 tam-per-card-t" @mouseover="aggd(ids[5])" :style="'background:' + fondod" @mouseout="volver()">
                <img src="@/assets/fotosdeperfil/Steve.jpg" alt="" class="perfil-tercera-fila aseis">
                <div class="text-center">
                    <h4>Steve Surichanqui</h4>
                    <h5 class="cargo" :class="{cargoHo : sobree}">I&D</h5>
                    <a href="https://www.linkedin.com/in/steve-surichaqui/" class="colorsTO">Linkedin</a>
                </div>
            </div>
            <div class="row flex-column align-items-center m-0 tam-per-card-t" @mouseover="agge(ids[6])" :style="'background:' + fondoe" @mouseout="volver()">
                <img src="@/assets/fotosdeperfil/Luz.jpg" alt="" class="perfil-tercera-fila asiete">
                <div class="text-center">
                    <h4>Luz Melgarejo</h4>
                    <h5 class="cargo" :class="{cargoHo : sobref}">IMPACTO SOCIAL</h5>
                    <a href="https://www.linkedin.com/in/luzmelgarejohuisa/" class="colorsTO">Linkedin</a>
                </div>
            </div>
              <div class="row flex-column align-items-center m-0 tam-per-card-t" @mouseover="aggf(ids[7])" :style="'background:' + fondof" @mouseout="volver()">
                <img src="@/assets/fotosdeperfil/Piero.jpg" alt="" class="perfil-tercera-fila aocho">
                <div class="text-center">
                    <h4>Daniella Rivero</h4>
                    <h5 class="cargo" :class="{cargoHo : sobreg}">I&D</h5>
                    <a href="https://www.linkedin.com/in/daniella-rivero-leveroni-37b955191" class="colorsTO">Linkedin</a>
                </div>
            </div>
              <div class="row flex-column align-items-center m-0 tam-per-card-t" @mouseover="aggg(ids[8])" :style="'background:' + fondog" @mouseout="volver()">
                <img src="@/assets/fotosdeperfil/Aaron.jpg" alt="" class="perfil-tercera-fila anueve">
                <div class="text-center">
                    <h4>Aaron Llican</h4>
                    <h5 class="cargo" :class="{cargoHo : sobrei}">I&D</h5>
                    <a href="https://www.linkedin.com/in/aaron-daniel-llican-diaz-537115208" class="colorsTO">Linkedin</a>
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
            fondoa:'#ffffff',
            fondob:'#ffffff',
            fondoc:'#ffffff',
            fondod:'#ffffff',
            fondoe:'#ffffff',
            fondof:'#ffffff',
            fondog:'#ffffff',
            fondoi:'#ffffff',
            sobre:false,
            sobrea:false,
            sobreb:false,
            sobrec:false,
            sobred:false,
            sobree:false,
            sobref:false,
            sobreg:false,
            sobrei:false

        }
    },
    methods:{
        agg(index){
            this.fondo = this.colores[0],
            this.sobre = true
        },
        aggi(index){
            this.fondoi = this.colores[1],
            this.sobrea= true
        },
        agga(index){
            this.fondoa = this.colores[2],
            this.sobreb= true
        },
        aggb(index){
            this.fondob = this.colores[3],
            this.sobrec= true
        },
        aggc(index){
            this.fondoc = this.colores[4],
            this.sobred= true
        },
        aggd(index){
            this.fondod = this.colores[5],
            this.sobree= true
        },
        agge(index){
            this.fondoe = this.colores[6],
            this.sobref= true
        },
        aggf(index){
            this.fondof = this.colores[7],
            this.sobreg= true
        },
        aggg(index){
            this.fondog = this.colores[8],
            this.sobrei= true
        },
        volver(){
            this.fondo = '#ffffff'
            this.fondoi = '#ffffff'
            this.fondoa = '#ffffff'
            this.fondob = '#ffffff'
            this.fondoc = '#ffffff'
            this.fondod = '#ffffff'
            this.fondoe = '#ffffff'
            this.fondof = '#ffffff'
            this.fondog = '#ffffff'
            this.sobre = false
            this.sobrea=false
            this.sobreb=false
            this.sobrec=false
            this.sobred=false
            this.sobree=false
            this.sobref=false
            this.sobreg=false
            this.sobrei=false
        }
    }
}
</script>
<style>
    .auno{
        border: solid 5px #D57521;
        border-radius: 100%;
        padding: 0.5rem;
        background: #fff;
    }
    .ados{
        border: solid 5px #89D841;
        border-radius: 100%;
        padding: 0.5rem;
        background: #fff;
    }
    .atres{
        border: solid 5px #D70000;
        border-radius: 100%;
        padding: 0.5rem;
        background: #fff;
    }
    .acuatro{
        border: solid 5px #cfc17c;
        border-radius: 100%;
        padding: 0.5rem;
        background: #fff;
    }
    .acinco{
        border: solid 5px #852DDD;
        border-radius: 100%;
        padding: 0.5rem;
        background: #fff;
    }
    .aseis{
        border: solid 5px #6275E6;
        border-radius: 100%;
        padding: 0.5rem;
        background: #fff;
    }
    .asiete{
        border: solid 5px #CC8A81;
        border-radius: 100%;
        padding: 0.5rem;
        background: #fff;
    }
    .aocho{
        border: solid 5px #C89700;
        border-radius: 100%;
        padding: 0.5rem;
        background: #fff;
    }
    .anueve{
        border: solid 5px #6CBDE4;
        border-radius: 100%;
        padding: 0.5rem;
        background: #fff;
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
        width: 16rem;
        height: 16rem;
    }
    .perfil-segunda-fila{
        border-radius: 100%;
        width: 14rem;
        height: 14rem;
    }
    .perfil-tercera-fila{
        border-radius: 100%;
        width: 13rem;
        height: 13rem;
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
    .tam-per{
        padding: 2rem;
        transition: 0.4s all ease;
    }
    .tam-per-card-t{
        width: 25%;
        padding: 2rem;
        transition: 0.4s all ease;
    }

    .tam-per-card-s{
        width: 33.33%;
        padding: 2rem;
        transition: 0.4s all ease;
    }
    .max-uno{
        max-width: 43%;
        margin: 0 auto!important;
    }
    .max-dos{
        max-width: 75%;
        margin: 0 auto!important;
    }
    @media only screen and (max-width: 320px){
        .tam-per-card-t {
            width: 100%;
            padding: 4rem;
            transition: 0.4s all ease;
        }
        .perfil-primera-fila {
            border-radius: 100%;
            width: 19rem;
            height: 19rem;
        }
        .perfil-segunda-fila {
            border-radius: 100%;
            width: 19rem;
            height: 19rem;
        }
        .perfil-tercera-fila {
            border-radius: 100%;
            width: 19rem;
            height: 19rem;
        }
        .tam-per-card-t {
            width: 100%;
            padding: 1rem;
            transition: 0.4s all ease;
        } 
        .max-fomulario {
            max-width: 30rem;
            margin: 0 auto;
            background: #3755E0;
            padding: 2rem;
            margin-top: -10rem;
        }
        .tam-equema {
            height: 20rem;
            width: 20rem;
            position: absolute;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: space-between;
            margin-left: -3rem;
            margin-top: -3rem;
        }
        .tam-equema {
            height: 21rem;
            width: 21rem;
            position: absolute;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: space-between;
            margin-left: -3rem;
            margin-top: -3rem;
        }
        .borde-animacion {
            width: 15rem;
            height: 15rem;
            border: dashed #fff;
            border-radius: 100%;
        }
    }
    @media only screen and (max-width: 450px) and (min-width: 321px){
        .tam-per-card-t {
            width: 100%;
            padding: 4rem;
            transition: 0.4s all ease;
        }
        .perfil-primera-fila {
            border-radius: 100%;
            width: 19rem;
            height: 19rem;
        }
        .perfil-segunda-fila {
            border-radius: 100%;
            width: 19rem;
            height: 19rem;
        }
        .perfil-tercera-fila {
            border-radius: 100%;
            width: 19rem;
            height: 19rem;
        }
        .tam-per-card-t {
            width: 100%;
            padding: 1rem;
            transition: 0.4s all ease;
        }
    }
    
    @media only screen and (max-width: 600px) and (min-width: 451px) {
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
        .tam-per-card-t{
            width: 100%;
            padding: 4rem;
            transition: 0.4s all ease;
        }
}
    @media only screen and (max-width: 768px) and (min-width: 601px){
        .color-contacto{
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            height: 20rem;
        }
        .tam-per-card-t{
            width: 100%;
            padding: 4rem;
            transition: 0.4s all ease;
        }
           .tam-per-card-s{
            width: 100%;
            padding: 4rem;
            transition: 0.4s all ease;
        }
        .perfil-segunda-fila {
            border-radius: 100%;
            width: 12rem;
            height: 12rem;
        }
        .perfil-primera-fila {
            border-radius: 100%;
            width: 15rem;
            height: 14rem;
        }
        .tam-per-card-t {
            width: 50%;
            padding: 4rem;
            transition: 0.4s all ease;
        }
        .perfil-tercera-fila {
            border-radius: 100%;
            width: 15rem;
            height: 15rem;
        }
     
    }
    @media only screen and (max-width: 1204px) and (min-width: 769px) {
             .perfil-segunda-fila {
                border-radius: 100%;
                width: 12rem;
                height: 12rem;
            }
            .perfil-primera-fila {
                border-radius: 100%;
                width: 15rem;
                height: 14rem;
            }
            .tam-per-card-t {
                width: 50%;
                padding: 4rem;
                transition: 0.4s all ease;
            }
            .perfil-tercera-fila {
                border-radius: 100%;
                width: 15rem;
                height: 15rem;
            }
    }
</style>