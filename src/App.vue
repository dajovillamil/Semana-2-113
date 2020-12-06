<template>
   <div id="app">

    <section-menu></section-menu>
    <section-banner></section-banner>
    <section-api></section-api>
    <team-card></team-card>


    <div>
    <p class="txt_c"> {{ titulo }} </p>
    <div class="fila" v-for='(item, index) of team' :key='index'>
      <div class="col-5">
        <TeamCard v-bind:member="item"></TeamCard>
      </div>    
    </div>
    </div>
    
    <site-footer></site-footer>

  </div>

</template>

<script>

import SectionMenu from './components/SectionMenu';
import SectionBanner from './components/SectionBanner';
import SectionApi from './components/SectionApi';
import TeamCard from './components/TeamCard';
import SiteFooter from './components/SiteFooter';


export default {
  name: 'App',
  components: {
    SectionMenu,
    SectionBanner,
    SectionApi,
    TeamCard,
    SiteFooter
  
  },
  
 data(){
    return{
        title: 'INTEGRANTES EQUIPO 113',
        team: [{
          codigo:1,
          nombre: 'Ana María Rodríguez Botero',
          descripcion: 'Edad 23 años, Ingeniera Física de la Universidad Nacional. Tengo 23 años. Me gusta leer, viajar y aprender.',
          rol: 'Desarrollador Backend y Frontend',
          image: "",
        },{
          codigo:2,
          nombre: 'Ariel Alfonso Angarita Leon',
          descripcion: 'Tecnologo ADSI del SENA. Tengo 41 años. Me encanta la tecnología, los videojuegos y ver series de TV. Trabajo como contratista independiente en TIC.',
          rol: 'Analista de Software',
          image: "",
        },{
          codigo:3,
          nombre: 'Hessler Nevin Inampuez López',
          descripcion: 'Estudiante de ingenieria civil de la Universidad de Nariño, tecnico laboral por competencias en sistemas. Tengo 28 años, como pasatiempo juego LoL y trabajo de manera independiente.',
          rol: 'Tester',
          image: "",
        },{
          codigo:4,
          nombre: 'David Johan Villamil Padilla',
          descripcion: 'Ingeniero industrial de 27 años egresado de la Universidad de Ibague, Actualmente milito como consultor de Bussines inteligence para Axity Colombia, estudio  Para el MINTIC a traves de imaster en el piloto.',
          rol: 'Arquitecto de Software',
          image: "",
        },
        ],
    }
  }
}

</script>

<style>
#app {
  
  text-align: center;
  
}
</style>
