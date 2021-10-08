<template>
<ul>
    <li><a href="#">Home</a></li>
    <li><a href="#">Projetos</a></li>
    <li><a href="#">Contato</a></li>
</ul>
</template>
<script>
export default{
    name:'Header'
}
</script>
<style scoped>
    ul{
        list-style: none;
        display: flex;
        background:#997;
        height: 30px;
    }
    li{
        margin-right: 10px;
        margin-top: 1%;
    }
    a{
        color: #DDD;
        text-decoration: none;
        transition: .5s.
    }
    a:hover{
        color:turquoise;
    }
</style>