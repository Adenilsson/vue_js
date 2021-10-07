<template>
<div>
  <PrimeiroComponente />
  <p>O dador de app é:{{testando}}</p>
  <LifeCycle/>
</div>
</template>
<script >
import PrimeiroComponente from './components/PrimeiroComponente.vue'
import LifeCycle from './components/LifeCycles.vue' 
  export default{
    name:'App',
    components:{
      PrimeiroComponente,
      LifeCycle
    },
    data(){
      return {
         testando: "teste de componente dentro de AppVue"
      }
     
    }
  }
</script>