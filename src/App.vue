<template>
<div>

  <PrimeiroComponente />
  <p>O dador de app é:{{testando}}</p>
  <LifeCycle/>
  <Pessoa/>
</div>
</template>
<script >
import PrimeiroComponente from './components/PrimeiroComponente.vue'
import LifeCycle from './components/LifeCycles.vue' 
import Pessoa from './components/Pessoa.vue' 

  export default{
    name:'App',
    components:{
      PrimeiroComponente,
      LifeCycle,
      Pessoa
     
    },
    data(){
      return {
         testando: "teste de componente dentro de AppVue"
      }
     
    }
  }
</script>