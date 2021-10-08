<template>
<p>TESTE DE FORMULARIO</p>
<form action="">
<div>
<InputText />
</div>
<div>
<InputText />
</div>
<div>
<Enviar />
</div>,
</form>
</template>
<script>
import InputText from './forms/InputText.vue'
import Enviar from './forms/Enviar.vue'
export default{
    name:'Formulario',
    components:{
        Enviar,
        InputText
        
    }
}
</script>