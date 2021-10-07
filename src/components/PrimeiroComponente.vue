<template>
<div>
    <h1> Olá Vue! </h1>
    <p>Meu nome é {{nome}}.</p>
    <p> Profissao:{{profissao}}.</p>
</div>
</template>


<script>
export default {
    name: 'PrimeiroComponente',
    data(){
        return{
            nome: "Adenilson",
            profissao:"Programador"
        }
    }
}
</script>