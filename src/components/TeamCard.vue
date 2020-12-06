<template>
    <div>
        <img v-bind:src= "member.image" alt="" class="team-imagenPerfil" >
        <h3 class="titulos"> {{member.codigo}} {{member.nombre}} </h3>
        <p class="parrafo"> {{ member.rol }} </p>
        <span class="descripcion"> {{ member.descripcion }} </span>
      
    </div>
</template>


<script>
export default {
  name: 'TeamCard',
  props: ['member']
}
</script>

<style>

.txt_c{
    font-size: 40px;
    text-align: center;
    background: rgba(247, 115, 27, 0.658);
    color:#243755;
}
.col-5 {
    max-width: 100%;
    height: 380px;
    text-align: justify;
    margin-bottom: 15px;
    border-radius: 0.7cm;
    background: #1f5a0d;
    margin: 5px;
}
.fila {
  width: 100%;
  margin-right: 0px;
  margin-left: 0px;
  display: block;
}
.titulos {
  text-align: center;
  color: aliceblue;
}
.parrafo {
  text-align: center;
  color: #cfc42a;
  font-size: 25px;
}
.tituloGrande{
  text-align: center;
}
img {
  border-style: groove;
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.team-imagenPerfil{
    height: 150px;
    width: 150px;
    border-radius: 2cm;
}
.descripcion {
  color: beige;
}
@media (min-width: 576px) {
  
  .fila {
    width: 44%;
    display: inline-block;
    margin-right: 23px;
    vertical-align: middle;
  }
  .col-5 {
    max-width: 100%;
    height: 525px;
    float: none;
  }
}
@media (min-width: 768px) {
  .fila {
    width: 44%;
    display: inline-block;
    margin-right: 28px;
    vertical-align: middle;
  }
  .col-5 {
    max-width: 96%;
    height: 420px;
    float: none;
  }
}
  
@media (min-width: 800px) {
  .fila {
    width: 30%;
    display: inline-block;
    margin-right: 23px;
    vertical-align: middle;
  }
  .col-5 {
    max-width: 96%;
    height: 550px;
    /* vertical-align: middle; */
    float: none;
  }
  .titulos {
    height: 99px;
  }
}
  
@media (min-width: 1000px) {
  .fila {
    width: 20%;
    display: inline-block;
    margin-right: 32px;
    vertical-align: middle;
  }
  .col-5 {
    max-width: 100%;
    height: 580px;
    /* vertical-align: middle; */
    float: none;
  }
    .titulos {
    height: 105px;
    font-size: 25px;
    vertical-align: middle;
    margin-top: 20px;
  }
    .parrafo{
    margin-top: 10px;
    font-size: 22px;
  }
}
@media (min-width: 1200px) {
  .fila {
    width: 17%;
    display: inline-block;
    margin-right: 32px;
    vertical-align: middle;
  }
  .col-5 {
    max-width: 100%;
    height: 550px;
    float: none;
    margin-left: 12px;
    vertical-align: middle;
  }

  .descripcion {
    vertical-align: sub;
  }
  .titulos {
    height: 105px;
    font-size: 25px;
    vertical-align: middle;
    margin-top: 20px;
  }
  .parrafo{
    margin-top: 10px;
    font-size: 22px;
  }
}

</style>
