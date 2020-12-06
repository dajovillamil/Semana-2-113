<template>
    <div>
        <footer class="footer">
        <div class = "informacion">
            <h4>INFORMACIÓN DEL SITIO WEB</h4>
            <div><label for="">Proyecto desarrollado por el Grupo 113 del ciclo 3 MinTic, en aras de adquirir conocimiento de programacion de paginas web, usando el pseudocódigo html. Estamos motivados al crecimiento personal y grupal de nuestra comunidad, entendemos que tomando como herramienta a la tecnologia nos ayudanran a fojar un mejor futuro para todos.</label></div>
            <div><label for="">En el siguiente link encontrará el desarrollo del reto: <a href="https://github.com/aaal79/semana-2-113.git"> Semana-2-113 en github </a> </label></div>
                       
        </div>
        
        <div class = "contacts">
            <h4>CONTACTOS</h4>
            <div><label for="">Ana María Rodríguez Botero. Desarrollador Backend-Frontend. anmrodriguezbo@unal.edu.co/3116676829</label></div>
            <div><label for="">Ariel Alfonso Angarita Leon. Analista de Software. aaal79@hotmail.com/3175038688</label></div>
            <div><label for="">Hessler Nevin Inampuez López. Tester. hesslernevin@gmail.com/3146433117</label></div>
            <div><label for="">David Johan Villamil Padilla. Arquitecto de Software. dajovillamil@gmail.com/3203297787</label></div>
                    
        </div>
        </footer>
    </div>
</template>

<script>
export default {
    name: 'SiteFooter',
}
</script>

<style>

.footer{
    color: rgb(5, 5, 5);
    bottom: 0;
    width: 100%;
    height: 40px;
    display: flex;
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    background-color: #D5EA7E;
    text-align: center;
    font-size: small;

}

.informacion{
    width: 100%;
    max-width: 50%;
  
}
            
.contacts{
    width: 100%;
    max-width: 50%;
    }

</style>
