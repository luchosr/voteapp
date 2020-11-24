<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" class="logo" >    
      
        <p><router-link to="/">Inicio</router-link>&nbsp;          
        <!-- <router-link to="/castBallot">Cast Ballot</router-link>&nbsp; -->
        <router-link to="/QueryAll">Consulta Todo</router-link></p>
        <router-link to="/queryWithQueryString">Consultar por Tipo</router-link>&nbsp;
        <router-link to="/queryByKey">Consultar por Clave</router-link>&nbsp;
        <router-link to="/getCurrentStanding">Obtener resultados de la encuesta</router-link>&nbsp;
      
      <router-view></router-view>
    </div>
</template>

<script>

export default {
  name: 'app'  
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.logo{
width: 20%;
}
.chart-wrapper {
  width: 100%;
  height: 700px;
}
.echarts {
  width: 100%;
  height: 100%;
}

#loader {
  position:fixed;
  padding-top: 250px;
}

.chart-wrapper {
  position:fixed;
  padding-left:32%;
}
</style>
