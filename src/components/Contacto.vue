<template>
    <div class="row justify-content-between m-0">
        <div class="col-md-6 fondo-contacto"></div>
        <div data-aos="fade-up"
     data-aos-anchor-placement="top-bottom" class="col-md-6 color-contacto">
            <h4 class="contacto-texto">Contacto</h4>
            <div>
                <p class="m-0 tipo-contacto">ASSISTIVE TECHNOLOGIES S.A.C</p>
                <p class="m-0 tipo-contacto">+51 987 582 891 / +51 981 227 430</p>
                <p class="m-0 tipo-contacto">piero.cosme.@utec.edu-pe</p>
            </div>
        </div>
        <div class="redes-contacto">
            <a href="#">
                <svg class="redes" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 78.41 78.41"><defs></defs><title>Recurso 14</title><g id="a1338500-ebe8-484b-957e-f18c4cb5a093" data-name="Capa 2"><g id="b368d840-ea7f-407a-8307-4938fcc8486b" data-name="Capa 1"><path d="M39.2,0A39.21,39.21,0,1,0,78.41,39.21,39.21,39.21,0,0,0,39.2,0"/><path d="M39.2,20.73A18.47,18.47,0,1,0,57.68,39.2,18.48,18.48,0,0,0,39.2,20.73"/><path class="a2ac4f77-9385-4a5e-9210-46c024a8004e" d="M39.2,20.73A18.47,18.47,0,1,0,57.68,39.2,18.48,18.48,0,0,0,39.2,20.73Z"/><path class="a0ae4e29-3ee1-46e6-bed7-6b8a76e0df95" d="M54.79,11.83a2.89,2.89,0,1,0,2.89,2.88,2.89,2.89,0,0,0-2.89-2.88"/><path class="b6301313-7e6b-4101-b6ab-3350417e2900" d="M54.79,11.83a2.89,2.89,0,1,0,2.89,2.88A2.89,2.89,0,0,0,54.79,11.83Z"/></g></g></svg>
            </a>
            <a href="#">
                <svg class="redes" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 80.76 80.76"><defs></defs><title>Recurso 15</title><g id="b13950cf-875f-4ee4-af75-2ce7ab097770" data-name="Capa 2"><g id="b1095c0a-26c3-4286-8bcf-b46304696775" data-name="Capa 1"><path d="M40.38,0A40.38,40.38,0,1,0,80.76,40.38,40.39,40.39,0,0,0,40.38,0"/><path class="b9df2987-16bc-421e-a217-dbed1c51eff1" d="M51.89,25.31a27.75,27.75,0,0,0-4.74-.52c-3.41,0-3.63,1.48-3.63,3.85v4.22H52l-.74,8.74H43.52V68.19H32.85V41.6H27.37V32.86h5.48v-5.4c0-7.41,3.48-11.55,12.22-11.55a37.34,37.34,0,0,1,8.15,1Z"/></g></g></svg>
            </a>
            <a href="#">
                <svg class="redes" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 81.08 81.07"><defs></defs><title>Recurso 16</title><g id="abc2721a-49a4-4563-ab8e-c36359278cb8" data-name="Capa 2"><g id="a0a489ff-ee15-4da5-be7f-9040129247df" data-name="Capa 1"><path d="M40.54,0A40.54,40.54,0,1,0,81.08,40.54,40.55,40.55,0,0,0,40.54,0"/><path class="addc4c4e-86e7-4f01-9a3f-e72fafec8b09" d="M26.88,19.87a3.19,3.19,0,0,1-3.44,3.32,3.22,3.22,0,0,1-3.26-3.32,3.3,3.3,0,0,1,3.39-3.38,3.21,3.21,0,0,1,3.31,3.38m-6,8.36h5.41V58H20.86Z"/><path class="addc4c4e-86e7-4f01-9a3f-e72fafec8b09" d="M35.24,36.28c0-3.07-.06-5.59-.24-8h4.79l.31,4.92h.12a11,11,0,0,1,9.84-5.6c4.11,0,10.51,2.46,10.51,12.67V58H55.16V40.83C55.16,36,53.38,32,48.27,32A7.68,7.68,0,0,0,41,37.57a8,8,0,0,0-.37,2.52V58H35.24Z"/></g></g></svg>
            </a>
        </div>
    </div>
</template>
<script>
export default {
    name:'Contacto'
}
</script>
<style>
    .fondo-contacto{
        background-image: url(../assets/fotosdeperfil/fondo.png);
        background-position: center center;
        background-repeat: no-repeat;
        background-size: cover;
        height: 50vh;
    }
    .color-contacto{
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
    }
    .tipo-contacto{
        font-size: 0.8rem;
        font-weight: bold;
    }
    .contacto-texto{
        font-weight: bold;
        margin-bottom: 2rem;
    }
    .a2ac4f77-9385-4a5e-9210-46c024a8004e,.b6301313-7e6b-4101-b6ab-3350417e2900{
        fill:none;stroke-miterlimit:10;
    }
    .a2ac4f77-9385-4a5e-9210-46c024a8004e{
        stroke:#fff;stroke-width:4px;
    }
    .a0ae4e29-3ee1-46e6-bed7-6b8a76e0df95{
        fill:#fff;
    }
    .b6301313-7e6b-4101-b6ab-3350417e2900{
        stroke:#000;stroke-width:0.75px;
    }
    .b9df2987-16bc-421e-a217-dbed1c51eff1{
        fill:#fff;
    }
    .addc4c4e-86e7-4f01-9a3f-e72fafec8b09{
        fill:#fff;
    }
    .redes-contacto{
        position: absolute;
        right: 3rem;
        height: 50vh;
        display: flex;
        align-items: flex-end;
        justify-content: space-between;
        margin-top: -2rem;
        width: 10rem;
    }
    .redes{
        width: 3rem;
    }
@media only screen and (max-width: 600px){ 
    .color-contacto{
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        height: 20rem;
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