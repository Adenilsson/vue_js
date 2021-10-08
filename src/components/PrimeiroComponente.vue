<template>
<div>
    <h1> Olá Vue! </h1>
    <p>Meu nome é {{nome}}.</p>
    <p> Profissao:{{profissao}}.</p>
    <MultiplosEvent />
</div>
</template>


<script>
import MultiplosEvent from './MultiplosEventos.vue'
export default {
    
    name: 'PrimeiroComponente',
    data(){
        return{
            nome: "Adenilson",
            profissao:"Programador"
        }
    },
    components:{
        MultiplosEvent

    }
}
</script>