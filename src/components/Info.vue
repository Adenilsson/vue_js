<template>
<div>
    <Picture />
    <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
    <p v-else>Não estou trabalhando no momento</p>
    <p>Utilizo as seguintes tecnologias: </p>
    <ul>
        <li>Javascript</li>
        <li>PHP</li>
        <li>Python</li>
        <li>Java</li>
        <li>C++</li>

    </ul>
    <div>
        <button @click="showEmail">{{texbooton}}</button>
    </div>
    <p v-show="mostrar_email">Mande uma mensagem para  {{email}}</p>
    <p>Para acessar meu portifólio <a v-bind:href="meu_link" target="_blank">meu link</a></p>
</div>
</template>

<script>
import Picture from './Picture'
export default{
    nome: 'Info',
    data(){
        return {
            esta_trabalhando: true,
            mostrar_email: false,
            email: 'adenilson@fairtek.com.br',
            meu_link:'https://google.com',
            texbooton:'Mostrar e-mail'
        }
    },
    components:{
        Picture
    },
    methods:{
        showEmail(){
            this.mostrar_email = !this.mostrar_email;
            if(!this.mostrar_email){
                this.texbooton = 'Mostrar e-mail'
            }else{
                this.texbooton ='Ocultar e-mail'
            }
        }
    }

}
</script>