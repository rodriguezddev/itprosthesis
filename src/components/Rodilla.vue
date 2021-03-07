<template>
    <div > 

        <div class="cont-color-dinamico" :style="'background:'+ objetoRodilla.color" style="padding-top: 0.55rem;">
        <h2 class="protesis col-md-5 ">PRÓTESIS</h2>
        <div>
            <ul class="row m-0 justify-content-around menu-rodilla p-0">
                <li class="item-lista">Accesible</li>
                <li class="item-lista">Modular</li>
                <li class="item-lista">Multifuncional</li>
                <li class="item-lista">Ligero</li>
            </ul>
            <div class="row align-items-center mr-0 ml-0 cont-rodilla-todo pb-4">
                <div class="row justify-content-around align-items-center mr-4 ml-0 col-md-5 no-mover">
                    <svg class="rodilla" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 467.97 480.21">
                    <defs></defs>
                    <g id="Capa_2" data-name="Capa 2">
                        <g id="Capa_7" data-name="Capa 7">
                            <path class="cls-1" @mouseover="cambiar(index[0])" @mouseleave="inicio()" d="M409.84,46.91V0H44.48S14.49.56,2,36.39c0,0-10.9,28.83,17.92,53.76L294.16,302.82S330,334.76,367.38,334H468V301.2H368.16s-25.31,1.23-57.64-26.43L37.08,62.1S29.29,57.43,34,42.63c0,0,3.9-9.35,11.69-9.35H291.82V46.52Z"/>
                            <path class="cls-1" @mouseover="cambiar(index[1])" @mouseleave="inicio()" d="M468,346.9v31.42H364.64s-68.71,2-120.43-44.33L25,164.54l20.65-25.32L261.44,306.71s42.84,39.73,101.27,39.73Z"/>
                            <path class="cls-1" @mouseover="cambiar(index[2])" @mouseleave="inicio()" d="M41.36,351.51v26.82H117.9s24.74-1.11,31.16-26.82c0,0,12.27-31.16-18.11-54.53L58.5,236.21l-17.14,18.9L115,317.62s12.86,9,9.35,24.15c0,0-3.12,10.13-11.69,10.13Z"/>
                            <rect class="cls-1" @mouseover="cambiar(index[4])" @mouseleave="inicio()" x="39.81" y="447.69" width="428.16" height="32.52"/>
                            <path class="cls-1" @mouseover="cambiar(index[3])" @mouseleave="inicio()" d="M253.89,373.67c-55.94,0-71.52,21.81-140.72,21.81H39.81v32.43l74-.06c51.42,0,95.82-21.35,140.08-21.35,50,0,85.06,19.79,131,19.79L468,427.91V395.48L384.52,394C335.05,394,301.56,373.67,253.89,373.67Z"/>
                            </g>
                        </g>
                    </svg>
                </div>
                <div class="col-md-5">
                    <div class=" bor-texto" :style="'border-left: 3px solid' +  objetoRodilla.colorFuente">
                        <div class="row justify-content-center  flex-column ml-4 mr-0">
                        <span class="font-title" v-html="objetoRodilla.name"></span>
                            <p class="font-protesis mt-4" :style="'color:' + objetoRodilla.colorFuente">
                                <span v-html="objetoRodilla.texto"></span>
                            </p>
                        </div>
                    </div>
                    <div v-html="objetoRodilla.esquema" class="row justify-content-center d-xl-flex d-lg-flex d-md-none d-none"> 
                            
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
    
</template>
<script>
export default {
    name:'Rodilla',
    data(){
        return {
            datosRodilla:[
                {
                    id:0,
                    name:'Quilla I',
                    color: '#F7E200',
                    texto:`Perfecta para el día a día, ir a tu trabajo, pasar tiempo con tu familia e incluso actividades de mediana exigencia física`,
                    colorFuente:'#000',
                    esquema:`
                        <svg class="ml-4 mr-4" xmlns="http://www.w3.org/2000/svg" width="8rem" height="8rem" viewBox="0 0 193.6 162.55"><defs></defs><g id="Capa_2" data-name="Capa 2"><g id="Capa_7" data-name="Capa 7"><path class="cls-card" d="M169.55,19.41V0H18.4S6,.23.84,15.06c0,0-4.51,11.92,7.41,22.23l113.44,88s14.83,13.21,30.3,12.89H193.6V124.61H152.31s-10.47.51-23.85-10.94l-113.12-88s-3.22-1.93-1.29-8.06c0,0,1.61-3.86,4.84-3.86H120.73v5.48Z"/><path class="cls-card" d="M35.73,124.73v11.1H67.39a14.44,14.44,0,0,0,12.89-11.1s5.08-12.89-7.49-22.56L42.82,77l-7.09,7.81,30.45,25.87s5.32,3.7,3.87,10c0,0-1.29,4.19-4.83,4.19Z"/><path class="cls-card" d="M105,140.11c-23.14,0-29.58,9-58.21,9H16.47v13.42l30.61,0c21.28,0,39.65-8.83,58-8.83,20.69,0,35.19,8.19,54.21,8.19l34.36.67V149.13l-34.52-.63C138.61,148.5,124.75,140.11,105,140.11Z"/></g></g></svg>
                        <svg class="ml-4 mr-4" xmlns="http://www.w3.org/2000/svg" width="8rem" height="8rem" viewBox="0 0 201.46 158.12"><defs></defs><g id="Capa_2" data-name="Capa 2"><g id="Capa_7" data-name="Capa 7"><path class="cls-card" d="M169.55,19.41V0H18.4S6,.23.84,15.06c0,0-4.51,11.92,7.41,22.23l113.44,88s14.83,13.21,30.3,12.89H193.6V124.61H152.31s-10.47.51-23.85-10.94l-113.12-88s-3.22-1.93-1.29-8.06c0,0,1.61-3.86,4.84-3.86H120.73v5.48Z"/><path class="cls-card" d="M35.73,124.73v11.1H67.39a14.44,14.44,0,0,0,12.89-11.1s5.08-12.89-7.49-22.56L42.82,77l-7.09,7.81,30.45,25.87s5.32,3.7,3.87,10c0,0-1.29,4.19-4.83,4.19Z"/><rect class="cls-card" x="24.33" y="144.67" width="177.13" height="13.45"/></g></g></svg>
                    `
                },
                 {
                    id:1,
                    name:'Quilla II',
                    color: '#66B42B',
                    texto:'Préparate para el siguiente nivel de actividades todoterreno. La curva pronunciada de la Quilla II esta diseñada para brindarte un mejor retorno de energía y evitar la fatiga excesiva después de un partido de fulbito, salir a correr y cualquier deporte que te propongas.',
                    colorFuente:'#424242;',
                    esquema:`
                        <svg class="ml-4 mr-4" xmlns="http://www.w3.org/2000/svg" width="8rem" height="8rem" viewBox="0 0 183.25 121.21"><defs></defs><g id="Capa_2" data-name="Capa 2"><g id="Capa_7" data-name="Capa 7"><path class="cls-card" d="M183.25,85.92v13H140.51s-28.43.85-49.82-18.33L0,10.47,8.54,0,97.81,69.29s17.73,16.44,41.9,16.44Z"/><path class="cls-card" d="M17.52,87.82v11.1H49.19a14.45,14.45,0,0,0,12.89-11.1s5.08-12.89-7.49-22.56l-30-25.14-7.09,7.82L48,73.8s5.32,3.71,3.87,10c0,0-1.29,4.19-4.84,4.19Z"/><rect class="cls-card" x="6.12" y="107.75" width="177.13" height="13.45"/></g></g></svg>
                        <svg class="ml-4 mr-4" xmlns="http://www.w3.org/2000/svg" width="8rem" height="8rem" viewBox="0 0 183.25 98.92"><defs></defs><g id="Capa_2" data-name="Capa 2"><g id="Capa_7" data-name="Capa 7"><path class="cls-card" d="M183.25,85.92v13H140.51s-28.43.85-49.82-18.33L0,10.47,8.54,0,97.81,69.29s17.73,16.44,41.9,16.44Z"/><path class="cls-card" d="M17.52,87.82v11.1H49.19a14.45,14.45,0,0,0,12.89-11.1s5.08-12.89-7.49-22.56l-30-25.14-7.09,7.82L48,73.8s5.32,3.71,3.87,10c0,0-1.29,4.19-4.84,4.19Z"/></g></g></svg>
                        <svg class="ml-4 mr-4" xmlns="http://www.w3.org/2000/svg" width="8rem" height="8rem" viewBox="0 0 185.74 121.09"><defs></defs><g id="Capa_2" data-name="Capa 2"><g id="Capa_7" data-name="Capa 7"><path class="cls-card" d="M183.25,85.92v13H140.51s-28.43.85-49.82-18.33L0,10.47,8.54,0,97.81,69.29s17.73,16.44,41.9,16.44Z"/><path class="cls-card" d="M17.52,87.82v11.1H49.19a14.45,14.45,0,0,0,12.89-11.1s5.08-12.89-7.49-22.56l-30-25.14-7.09,7.82L48,73.8s5.32,3.71,3.87,10c0,0-1.29,4.19-4.84,4.19Z"/><path class="cls-card" d="M97.17,98.64c-23.14,0-29.59,9-58.21,9H8.61v13.42l30.61,0c21.27,0,39.64-8.83,58-8.83,20.69,0,35.19,8.19,54.21,8.19l34.36.67V107.67L151.22,107C130.75,107,116.89,98.64,97.17,98.64Z"/></g></g></svg>
                    `
                },
                 {
                    id:2,
                    name:'TACON',
                    color: '#DD3B00',
                    texto:`El mejor complemento para esas actividades que requieren de saltos, trotes, o para una larga caminata.`,
                    colorFuente:'#424242;',
                    esquema:`
                        <svg class="ml-4 mr-4" xmlns="http://www.w3.org/2000/svg"  width="8rem" height="8rem" viewBox="0 0 147.03 97.25"><defs></defs><g id="Capa_2" data-name="Capa 2"><g id="Capa_7" data-name="Capa 7"><path class="cls-card" d="M147,68.94V79.36H112.74s-22.81.68-40-14.71L0,8.4,6.85,0,78.48,55.6S92.7,68.78,112.1,68.78Z"/><path class="cls-card" d="M14.06,70.46v8.91H39.47a11.59,11.59,0,0,0,10.34-8.91s4.07-10.34-6-18.1l-24-20.17-5.69,6.28L38.5,59.22s4.26,3,3.1,8c0,0-1,3.36-3.88,3.36Z"/><rect class="cls-card" x="4.91" y="86.46" width="142.12" height="10.79"/></g></g></svg>
                        <svg class="ml-4 mr-4" xmlns="http://www.w3.org/2000/svg" width="7rem" height="7rem" viewBox="0 0 155.33 130.42"><defs></defs><g id="Capa_2" data-name="Capa 2"><g id="Capa_7" data-name="Capa 7"><path class="cls-card" d="M136,15.57V0H14.76S4.81.19.67,12.08c0,0-3.62,9.57,6,17.84l91,70.6s11.9,10.6,24.31,10.34h33.38V100H122.21s-8.41.41-19.14-8.77L12.31,20.61s-2.59-1.55-1-6.46c0,0,1.3-3.1,3.88-3.1H96.87v4.39Z"/><path class="cls-card" d="M28.67,100.08V109h25.4a11.61,11.61,0,0,0,10.35-8.9s4.07-10.34-6-18.1l-24-20.17-5.69,6.27L53.1,88.83s4.27,3,3.11,8c0,0-1,3.36-3.88,3.36Z"/><path class="cls-card" d="M84.27,112.41c-18.56,0-23.74,7.25-46.71,7.25H13.21v10.76l24.57,0c17.07,0,31.8-7.09,46.49-7.09,16.6,0,28.24,6.57,43.5,6.57l27.56.54V119.66l-27.69-.51C111.22,119.15,100.1,112.41,84.27,112.41Z"/></g></g></svg>
                        <svg class="ml-4 mr-4" xmlns="http://www.w3.org/2000/svg" width="7rem" height="7rem" viewBox="0 0 161.64 126.87"><defs></defs><g id="Capa_2" data-name="Capa 2"><g id="Capa_7" data-name="Capa 7"><path class="cls-card" d="M136,15.57V0H14.76S4.81.19.67,12.08c0,0-3.62,9.57,6,17.84l91,70.6s11.9,10.6,24.31,10.34h33.38V100H122.21s-8.41.41-19.14-8.77L12.31,20.61s-2.59-1.55-1-6.46c0,0,1.3-3.1,3.88-3.1H96.87v4.39Z"/><path class="cls-card" d="M28.67,100.08V109h25.4a11.61,11.61,0,0,0,10.35-8.9s4.07-10.34-6-18.1l-24-20.17-5.69,6.27L53.1,88.83s4.27,3,3.11,8c0,0-1,3.36-3.88,3.36Z"/><rect class="cls-card" x="19.52" y="116.07" width="142.12" height="10.79"/></g></g></svg>
                        <svg class="ml-4 mr-4" xmlns="http://www.w3.org/2000/svg" width="7rem" height="7rem" viewBox="0 0 147.03 79.37"><defs></defs><g id="Capa_2" data-name="Capa 2"><g id="Capa_7" data-name="Capa 7"><path class="cls-card" d="M147,68.94V79.36H112.74s-22.81.68-40-14.71L0,8.4,6.85,0,78.48,55.6S92.7,68.78,112.1,68.78Z"/><path class="cls-card" d="M14.06,70.46v8.91H39.47a11.59,11.59,0,0,0,10.34-8.91s4.07-10.34-6-18.1l-24-20.17-5.69,6.28L38.5,59.22s4.26,3,3.1,8c0,0-1,3.36-3.88,3.36Z"/></g></g></svg>
                        <svg class="ml-4 mr-4" xmlns="http://www.w3.org/2000/svg" width="7rem" height="7rem"viewBox="0 0 149.03 97.15"><defs></defs><g id="Capa_2" data-name="Capa 2"><g id="Capa_7" data-name="Capa 7"><path class="cls-card" d="M147,68.94V79.36H112.74s-22.81.68-40-14.71L0,8.4,6.85,0,78.48,55.6S92.7,68.78,112.1,68.78Z"/><path class="cls-card" d="M14.06,70.46v8.91H39.47a11.59,11.59,0,0,0,10.34-8.91s4.07-10.34-6-18.1l-24-20.17-5.69,6.28L38.5,59.22s4.26,3,3.1,8c0,0-1,3.36-3.88,3.36Z"/><path class="cls-card" d="M78,79.15c-18.57,0-23.74,7.24-46.71,7.24H6.9V97.15l24.57,0c17.07,0,31.81-7.08,46.5-7.08,16.59,0,28.23,6.57,43.49,6.57l27.57.53V86.39l-27.7-.51C104.91,85.88,93.79,79.15,78,79.15Z"/></g></g></svg>
                    `
                },
                 {
                    id:3,
                    name:'PLANTA CURVA',
                    color: '#E58300',
                    texto:`Experimenta un mayor retorno de energía con la curvatura de la planta y alístate para las actividades más exigentes`,
                    colorFuente:'#424242;',
                    esquema:`
                        <svg class="ml-4 mr-4" width="10rem" height="10rem" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 185.74 121.09"><defs></defs><g id="Capa_2" data-name="Capa 2"><g id="Capa_7" data-name="Capa 7"><path class="cls-card" d="M183.25,85.92v13H140.51s-28.43.85-49.82-18.33L0,10.47,8.54,0,97.81,69.29s17.73,16.44,41.9,16.44Z"/><path class="cls-card" d="M17.52,87.82v11.1H49.19a14.45,14.45,0,0,0,12.89-11.1s5.08-12.89-7.49-22.56l-30-25.14-7.09,7.82L48,73.8s5.32,3.71,3.87,10c0,0-1.29,4.19-4.84,4.19Z"/><path class="cls-card" d="M97.17,98.64c-23.14,0-29.59,9-58.21,9H8.61v13.42l30.61,0c21.27,0,39.64-8.83,58-8.83,20.69,0,35.19,8.19,54.21,8.19l34.36.67V107.67L151.22,107C130.75,107,116.89,98.64,97.17,98.64Z"/></g></g></svg>
                        <svg class="ml-4 mr-4" width="10rem" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 193.6 162.55"><defs></defs><g id="Capa_2" data-name="Capa 2"><g id="Capa_7" data-name="Capa 7"><path class="cls-card" d="M169.55,19.41V0H18.4S6,.23.84,15.06c0,0-4.51,11.92,7.41,22.23l113.44,88s14.83,13.21,30.3,12.89H193.6V124.61H152.31s-10.47.51-23.85-10.94l-113.12-88s-3.22-1.93-1.29-8.06c0,0,1.61-3.86,4.84-3.86H120.73v5.48Z"/><path class="cls-card" d="M35.73,124.73v11.1H67.39a14.44,14.44,0,0,0,12.89-11.1s5.08-12.89-7.49-22.56L42.82,77l-7.09,7.81,30.45,25.87s5.32,3.7,3.87,10c0,0-1.29,4.19-4.83,4.19Z"/><path class="cls-card" d="M105,140.11c-23.14,0-29.58,9-58.21,9H16.47v13.42l30.61,0c21.28,0,39.65-8.83,58-8.83,20.69,0,35.19,8.19,54.21,8.19l34.36.67V149.13l-34.52-.63C138.61,148.5,124.75,140.11,105,140.11Z"/></g></g></svg>
                    `
                },
                 {
                    id:4,
                    name:'PLANTA PLANA',
                    color: '#77D9FF',
                    texto:`Este elemento te dará una mejor sensación de balance y seguridad, perfecto para reuniones sociales, para el día a día o para ir al trabajo `,
                    colorFuente:'#424242;',
                    esquema:`
                        <svg class="ml-4 mr-4" width="10rem" height="10rem" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 183.25 121.21"><defs></defs><g id="Capa_2" data-name="Capa 2"><g id="Capa_7" data-name="Capa 7"><path class="cls-card" d="M183.25,85.92v13H140.51s-28.43.85-49.82-18.33L0,10.47,8.54,0,97.81,69.29s17.73,16.44,41.9,16.44Z"/><path class="cls-card" d="M17.52,87.82v11.1H49.19a14.45,14.45,0,0,0,12.89-11.1s5.08-12.89-7.49-22.56l-30-25.14-7.09,7.82L48,73.8s5.32,3.71,3.87,10c0,0-1.29,4.19-4.84,4.19Z"/><rect class="cls-card" x="6.12" y="107.75" width="177.13" height="13.45"/></g></g></svg>
                        <svg class="ml-4 mr-4" width="10rem" height="10rem" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 201.46 158.12"><defs></defs><g id="Capa_2" data-name="Capa 2"><g id="Capa_7" data-name="Capa 7"><path class="cls-card" d="M169.55,19.41V0H18.4S6,.23.84,15.06c0,0-4.51,11.92,7.41,22.23l113.44,88s14.83,13.21,30.3,12.89H193.6V124.61H152.31s-10.47.51-23.85-10.94l-113.12-88s-3.22-1.93-1.29-8.06c0,0,1.61-3.86,4.84-3.86H120.73v5.48Z"/><path class="cls-card" d="M35.73,124.73v11.1H67.39a14.44,14.44,0,0,0,12.89-11.1s5.08-12.89-7.49-22.56L42.82,77l-7.09,7.81,30.45,25.87s5.32,3.7,3.87,10c0,0-1.29,4.19-4.83,4.19Z"/><rect class="cls-card" x="24.33" y="144.67" width="177.13" height="13.45"/></g></g></svg>
                    `
                }
            ],
            index:[0,1,2,3,4],
            objetoRodilla:{},
            reinicio:{
                name:`<svg xmlns="http://www.w3.org/2000/svg" class="leg" viewBox="0 0 564.05 179.45"><defs></defs><g id="Capa_2" data-name="Capa 2"><g id="Capa_6" data-name="Capa 6"><path class="cls-leg" d="M91.19,162.76H0v-144H7.93V155.87H91.19Z"/><path class="cls-leg" d="M205.53,162.76H114.34v-144h89.1v6.68H122.27v62h76.37v6.68H122.27v61.76h83.26Z"/><path class="cls-leg" d="M344.91,97.24v65.52h-7.3V127.91l-4.8,13.36c-11.06,17.31-28.8,24.41-46.74,24.41-37.77,0-63.65-28.8-63.65-74.49,0-44.66,28.59-75.33,67.61-75.33,32.76,0,50.71,20.24,55.3,46.53l.41,2.09h-7.93l-.41-2.09c-4.59-22.74-20.66-39.65-48.2-39.65-30.89,0-58,24.84-58,68,0,44.86,24.62,68,55.5,68,22.12,0,50.29-15,50.29-54.67H292.12V97.24Z"/><path class="cls-2" d="M414.39,0C399,25.46,390.18,57.59,390.18,89.73S399,154,414.39,179.45H405c-15.23-22.95-24.83-56.76-24.83-89.72S389.77,23,405,0Z"/><path class="cls-leg" d="M448.55,28.59c0,4.8-3,8.76-7,8.76-3.81,0-7-4-7-8.76,0-5,3.15-8.77,7-8.77C445.57,19.82,448.55,23.58,448.55,28.59Zm-12.1,134.17V52.37h10.28V162.76Z"/><path class="cls-leg" d="M497.43,132.5c0,4.59,0,6.89.21,9.81.83,10.64,5.42,13.35,20.24,11.48v9.59a71.58,71.58,0,0,1-13.36,1.05c-12.31,0-18.78-5.43-19.82-17.53-.21-3.76-.21-7.93-.21-14.19V63.23H470.3v-10h14.19V28.8h12.94V53.21H518.5v10H497.43Z"/><path class="cls-2" d="M540.07,5.62c14.71,22.16,24,54.8,24,86.63s-9.27,64.46-24,86.62h-8.86c14.71-24.57,23.17-55.6,23.17-86.62s-8.46-62-23.17-86.63Z"/></g></g></svg>`,
                color: '#3755E0;',
                texto:`Nuestra prótesis <span><svg xmlns="http://www.w3.org/2000/svg" class="leg-rodilla" viewBox="0 0 564.05 179.45"><defs></defs><g id="Capa_2" data-name="Capa 2"><g id="Capa_6" data-name="Capa 6"><path class="cls-leg" d="M91.19,162.76H0v-144H7.93V155.87H91.19Z"/><path class="cls-leg" d="M205.53,162.76H114.34v-144h89.1v6.68H122.27v62h76.37v6.68H122.27v61.76h83.26Z"/><path class="cls-leg" d="M344.91,97.24v65.52h-7.3V127.91l-4.8,13.36c-11.06,17.31-28.8,24.41-46.74,24.41-37.77,0-63.65-28.8-63.65-74.49,0-44.66,28.59-75.33,67.61-75.33,32.76,0,50.71,20.24,55.3,46.53l.41,2.09h-7.93l-.41-2.09c-4.59-22.74-20.66-39.65-48.2-39.65-30.89,0-58,24.84-58,68,0,44.86,24.62,68,55.5,68,22.12,0,50.29-15,50.29-54.67H292.12V97.24Z"/><path class="cls-2" d="M414.39,0C399,25.46,390.18,57.59,390.18,89.73S399,154,414.39,179.45H405c-15.23-22.95-24.83-56.76-24.83-89.72S389.77,23,405,0Z"/><path class="cls-leg" d="M448.55,28.59c0,4.8-3,8.76-7,8.76-3.81,0-7-4-7-8.76,0-5,3.15-8.77,7-8.77C445.57,19.82,448.55,23.58,448.55,28.59Zm-12.1,134.17V52.37h10.28V162.76Z"/><path class="cls-leg" d="M497.43,132.5c0,4.59,0,6.89.21,9.81.83,10.64,5.42,13.35,20.24,11.48v9.59a71.58,71.58,0,0,1-13.36,1.05c-12.31,0-18.78-5.43-19.82-17.53-.21-3.76-.21-7.93-.21-14.19V63.23H470.3v-10h14.19V28.8h12.94V53.21H518.5v10H497.43Z"/><path class="cls-2" d="M540.07,5.62c14.71,22.16,24,54.8,24,86.63s-9.27,64.46-24,86.62h-8.86c14.71-24.57,23.17-55.6,23.17-86.62s-8.46-62-23.17-86.63Z"/></g></g></svg></span> 
                        está diseñada para que estés preparado ante cualquier ocasión. La diversidad de configuraciones le ofrece al usuario la posibilidad de decidir el tipo de prótesis que requiere según la actividad que desempeñará. Con <span><svg xmlns="http://www.w3.org/2000/svg" class="leg-rodilla" viewBox="0 0 564.05 179.45"><defs></defs><g id="Capa_2" data-name="Capa 2"><g id="Capa_6" data-name="Capa 6"><path class="cls-leg" d="M91.19,162.76H0v-144H7.93V155.87H91.19Z"/><path class="cls-leg" d="M205.53,162.76H114.34v-144h89.1v6.68H122.27v62h76.37v6.68H122.27v61.76h83.26Z"/><path class="cls-leg" d="M344.91,97.24v65.52h-7.3V127.91l-4.8,13.36c-11.06,17.31-28.8,24.41-46.74,24.41-37.77,0-63.65-28.8-63.65-74.49,0-44.66,28.59-75.33,67.61-75.33,32.76,0,50.71,20.24,55.3,46.53l.41,2.09h-7.93l-.41-2.09c-4.59-22.74-20.66-39.65-48.2-39.65-30.89,0-58,24.84-58,68,0,44.86,24.62,68,55.5,68,22.12,0,50.29-15,50.29-54.67H292.12V97.24Z"/><path class="cls-2" d="M414.39,0C399,25.46,390.18,57.59,390.18,89.73S399,154,414.39,179.45H405c-15.23-22.95-24.83-56.76-24.83-89.72S389.77,23,405,0Z"/><path class="cls-leg" d="M448.55,28.59c0,4.8-3,8.76-7,8.76-3.81,0-7-4-7-8.76,0-5,3.15-8.77,7-8.77C445.57,19.82,448.55,23.58,448.55,28.59Zm-12.1,134.17V52.37h10.28V162.76Z"/><path class="cls-leg" d="M497.43,132.5c0,4.59,0,6.89.21,9.81.83,10.64,5.42,13.35,20.24,11.48v9.59a71.58,71.58,0,0,1-13.36,1.05c-12.31,0-18.78-5.43-19.82-17.53-.21-3.76-.21-7.93-.21-14.19V63.23H470.3v-10h14.19V28.8h12.94V53.21H518.5v10H497.43Z"/><path class="cls-2" d="M540.07,5.62c14.71,22.16,24,54.8,24,86.63s-9.27,64.46-24,86.62h-8.86c14.71-24.57,23.17-55.6,23.17-86.62s-8.46-62-23.17-86.63Z"/></g></g></svg></span> 
                        estarás preparado para ir al trabajo, pasar un día familiar o incluso hacer el deporte que más te guste`,
                colorFuente:'#fff'
            }
        }
    },
    methods: {
        cambiar(index){
            console.log(index)
            this.objetoRodilla = this.datosRodilla[index]
            
        },
        inicio(){
            this.objetoRodilla = this.reinicio
        }
    },
    created(){
        this.objetoRodilla = this.reinicio
    }
}
</script>
<style>
    .protesis{
        margin-left: 3rem;
        font-size: 2.8rem;
        padding: 0;
        margin-bottom: 1.3rem;
        padding-top: 2rem;
        color: #ffffff;
    }
    .protesis::after{
        content: '';
        display: block;
        height: 0.2rem;
        width: 22rem;
        background-color:   rgb(255, 255, 255);
        margin-left:-3.6rem;
    }
    .menu-rodilla {
        color: #ffffff;
        font-size: 1.5rem;
    }
    .font-title{
        font-size: 4rem;
        transition: 0.4s all ease;
        color: #424242;
    }
    .cls-1{
        fill:#fff;
    }
    .cls-1:hover{
        fill:#000;
    }
    .rodilla{
        width: 17rem;
    }
  
    .cls-leg{
        fill:#fff;
    }
    .cls-2{
        fill:#dd3b00;
    }
    .leg{
        width: 18rem;
    }
    .leg-rodilla{
        width: 4rem;
    }
    .font-protesis{
        font-size: 1rem;
        color: #fff;
        transition: 0.4s all ease;
        text-align: justify
    }
    .bor-texto{
        border-left: 3px solid #fff;
    }
    .no-mover{
        height: 32rem;
    }
    /*valores dinamicos*/
    .cont-color-dinamico{
        background: #3755E0;
        transition: 0.4s all ease;
        padding-bottom: 5rem;
    }

    .cls-card{
        fill:#424242;
    }


@media only screen and (max-width: 600px){ 
    .leg{
        width: 15rem;
    }
    .font-protesis{
        font-size: 1rem;
        color: #fff;
        transition: 0.4s all ease;
    }
    .font-title{
        font-size: 2rem;
        transition: 0.4s all ease;
        color: #424242;
    }
    .item-lista{
        font-size: 1rem;
    }
}
@media only screen and (max-width: 768px) {
    .leg {
        width: 19rem;
    }
    .item-lista {
        font-size: 1.2rem;
        margin-bottom: 2rem;
    }
}
@media only screen and (max-width: 1440){ 
    .no-mover{
        height: 40rem;
    }
}
</style>