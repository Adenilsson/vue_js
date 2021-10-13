<template>
   
    <img :src="avatar " :alt="descricao">
    <Teste />
    <MudarImagem  @mudar-imagem="trocarImagem" />
    
</template>
<script>
import  MudarImagem from './MudarImagem.vue';
import Teste from './Teste.vue'
    export default{
        name:'Picture',
        data(){
            return{
                avatar:'/img/user.jpg',
                descricao: 'Adenilson'
            }
        },
        components:{
            MudarImagem
        },
        methods:{
            trocarImagem(){
                 this.avatar ="/img/user-avatar.png"
            }
        }
    }
</script>