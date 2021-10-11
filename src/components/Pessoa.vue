<template>
<div>
    <h2>Esta é a descrição da pessoa {{nome}}</h2>
    <Info :email="email" :estaTrabalhando=true />
    <Formulario />
    
</div>
</template>
<script>
import Info from './Info'
import Formulario from './Formulario'
export default {
    name: 'Pessoa',
    components: {
        Info,
        Formulario
    },

    data(){
        return{
             nome: 'Primeira pessoa',
             email:'Adenilson@email.com5'
        }
    }
    
}
</script>