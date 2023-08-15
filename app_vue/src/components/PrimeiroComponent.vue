<template>
    <div>
        <h1>Olá Vue!</h1>
        <p>meu nome é {{ name }} e sou {{ proff }}</p>
    </div>
</template>

<script>
    export default {
        name: "PrimeiroCompoment",
        data(){
            return {
                name: "Souzinha",
                proff: "Desenvolvedor Full Stack"
            }
        }
    }
</script>