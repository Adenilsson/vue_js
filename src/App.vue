<template>
<div>
  <Header :esta_logado ="true"/>
  <PrimeiroComponente />
  <p>O dador de app é:{{testando}}</p>
  <LifeCycle/>
  <Pessoa/>
  <Reutilizado />
  <Reutilizado />
  <Reutilizado />
  <Reutilizado />
</div>
</template>
<script >
import PrimeiroComponente from './components/PrimeiroComponente.vue'
import LifeCycle from './components/LifeCycles.vue' 
import Pessoa from './components/Pessoa.vue' 
import Header from './components/Header.vue' 
import Reutilizado from './components/Reutilizado.vue'
  export default{
    name:'App',
    components:{
      PrimeiroComponente,
      LifeCycle,
      Pessoa,
      Header,
      Reutilizado
     
    },
    data(){
      return {
         testando: "teste de componente dentro de AppVue"
      }
     
    }
  }
</script>

<style>
body{
  background-color:#333;
  color:#fff;
}
a{
  color:red;
}
.teste{
  background-color: blue;
}
</style>



