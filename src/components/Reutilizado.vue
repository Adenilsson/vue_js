<template>
<div>
<button @click="ativado">{{mensagem}}</button>

<span>{{estado}}</span>
</div>
</template>
<script>
export default{
    name:'Reutilizado',
    data(){
        return {
            ativa: true,
            mensagem:'Ativar',
            estado: 'Desativado'
        }
    },
    methods:{
        ativado(){
            if(!this.ativa){
                this.ativa =!this.ativa
                this.mensagem = 'Ativar'
                this.estado = 'Desativado'
            }else{
                this.ativa =!this.ativa
                this.mensagem = 'Desativar'
                this.estado = 'Ativado'
               
            }
        }
    }
}
</script>
<style scoped>
div{padding:10px;
}
span{padding:10px;}
</style>