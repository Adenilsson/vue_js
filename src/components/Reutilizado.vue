<template>
<button @click="ativado">{{mensagem}}</button>

<p>{{estado}}</p>
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