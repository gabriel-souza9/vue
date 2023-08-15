
<template>
    <h1>Meu nome é: {{ name }} </h1>
</template>

<script>
    export default {
        name: "LifeCycle",
        data(){
            return {
                name: "Ainda não sei"
            }
        },
        created(){
            this.name = "Gabriel"
        },
        mounted(){
            this.name = "Souzinha"
        }
        
    }
</script>