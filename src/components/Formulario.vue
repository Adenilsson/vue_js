<template>
<p>TESTE DE FORMULARIO</p>
<p v-if="form_enviado">Nome digitado é {{name}}</p>
<p v-if="form_enviado">Email informado {{email}}</p>
<form action="" @submit="enviarFormulario($event)">
<div>
<input type="text" v-model="name">
</div>
<div>
<input type="text" v-model="email">
</div>
<div>
<input type="submit" value="Enviar" @click="dados_enviados">
</div>,
</form>
</template>
<script>
import InputText from './forms/InputText.vue'
import Enviar from './forms/Enviar.vue'
export default{
    name:'Formulario',
    data(){
        return{
            name: '',
            email:'',
            enviar: false,
            form_enviado: false
        }
    },
    components:{
        Enviar,
        InputText
        
    },
    methods:{
        enviarFormulario(e){
            e.preventDefault();

            const name=  this.name;
            const email =  this.email;
            console.log('enviarFormulario',name, email);
        },
        dados_enviados(){
            if(this.enviar){
                this.form_enviado = false;
            }else{
                this.form_enviado = true;
            }
        }
    }
}
</script>