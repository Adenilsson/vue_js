<template>
<div>
    <h2>Esta é a descrição da pessoa {{nome}}</h2>
    <Info />
</div>
</template>
<script>
import Info from './Info'

export default {
    nome: 'Pessoa',
    components: {
        Info
    },
    data(){
        return{
             nome: 'Primeira pessoa'
        }
    }
    
}
</script>