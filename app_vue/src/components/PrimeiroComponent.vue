<template>
    <div>
        <h1>Olá Vue!</h1>
        <p>meu nome é {{ name }} e sou {{ proff }}</p>
        <MultiplosEventos />
    </div>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue';
    export default {
        name: "PrimeiroCompoment",
        components: {
            MultiplosEventos
        },
        data(){
            return {
                name: "Souzinha",
                proff: "Desenvolvedor Full Stack"
            }
        }
    }
</script>