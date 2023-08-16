<template>
<div>
    <h2>Está é a descrição da pessoa {{ nome }}</h2>
    <Info />
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
            nome: "Gabriel"
        }
    }
}
</script>
