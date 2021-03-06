<template>
    <div class="fondo-contentdor-fomulario">
        <div data-aos="fade-up" class="max-fomulario">
            <h3 class="text-center texto-form aaa">¿Desea ser beneficiado?</h3>
            <form 
               @submit.prevent="" class="row m-0 flex-column align-items-end">
                <label class="texto-form">Déjanos tu datos y uno de nuestros asesores se comunicarán contigo</label>
                <div class="row flex-column m-0 w-100">
                    <input type="text" v-model="nombre" placeholder="Nombre" class="input-form">
                    <input type="text" v-model="telefono" placeholder="Teléfono" class="input-form">
                    <input type="text" v-model="correo" placeholder="Correo" class="input-form">
                    <input type="text" v-model="amputacion" placeholder="Tipo de amputacion" class="input-form">
                    <input type="text" v-model="ocupacion" placeholder="Ocupación" class="input-form">
                </div>
                <button type="submit" @click="sendEmail" class="boton-form mt-4 pt-2 pb-2 pl-3 pr-3">Enviar</button>
            </form>
        </div>
    </div>
</template>
<script>
import emailjs from 'emailjs-com';
export default {
    name:'Beneficiados',
    data(){
       return{
            nombre:'',
            telefono:'',
            correo:'',
            amputacion:'',
            ocupacion:''
       }

    },
    created(){
       
        },
    methods: {
          sendEmail() {
              console.log(this.nombre, this.telefono, this.correo, this.amputacion, this.ocupacion)
               emailjs.init("user_Cpgc30JWe1k6Pr7DyHBWC");
               var mensaje = 'Lorem soul' + this.telefono + this.correo + this.amputacion + this.ocupacion
                            
            try {
                emailjs.send( 'service_uv7vfbe' , 'template_k75vbzl', {
                nombre: this.nombre,
                mensaje: mensaje
                })
        } catch(error) {
            console.log({error})
        }
        // Reset form field
        this.nombre = ''
        this.telefono = ''
        this.correo = ''
        this.amputacion = ''
        this.ocupacion = ''
        },
    },
}
</script>
<style>
    .max-fomulario{
        max-width: 30rem;
        margin:0 auto;
        background: #3755E0;
        padding: 3rem;
        margin-top: -10rem;
    }
    .fondo-contentdor-fomulario{
        background: #DD3B00;
        width: 100%;
        padding: 3rem;
    }
    .aaa{
        font-weight: 700;
    }
    .texto-form{
        color:#fff;
    }
    .input-form{
        background: transparent;
        border: none;
        border-bottom: solid #fff 1px;
        color: #fff;
        padding: 1rem;
    }
    .input-form::placeholder {
        color: #fff;
        font-size: 1rem;
    }
    .input-form:focus{
        outline: none;
        border-bottom: 2px solid #fff;
    }
    .boton-form{
        border:none;
        font-weight: bold;
        background: #F7E200; 
    }
@media only screen and (max-width: 600px){ 
    .fondo-contentdor-fomulario {
        background: #DD3B00;
        width: 100%;
        padding: 1rem;
    }
    .texto-form{
        text-align: center;
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
}
@media only screen and (max-width: 768px) {

}
</style>