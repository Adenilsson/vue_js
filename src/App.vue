<template>
<div>
  <Header />
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
import Header from './components/Header.vue' 
  export default{
    name:'App',
    components:{
      PrimeiroComponente,
      LifeCycle,
      Pessoa,
      Header
     
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



