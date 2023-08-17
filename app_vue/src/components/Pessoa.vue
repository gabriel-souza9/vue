<template>
<div>
    <h2>Está é a descrição da pessoa {{ nome }}</h2>
    <Info :email="email"/>
</div>
</template>

<script>
import Info from '../components/Info.vue';


export default {
    name: "Pessoa",
    components: {
        Info
    },
    data(){
        return {
            nome: "Gabriel",
            email: "souzinha@gmail.com/lindinho"
        }
    }
}
</script>
