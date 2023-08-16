<template>
    <div>
        <button @click="primeiro(txt1), segundo(txt2)">Ativar múltiplos eventos</button>
        <p>{{ multiplos_eventos }}</p>
    </div>
</template>

<script>
    export default {
        name: "MultiplosEventos",
        data(){
            return {
                multiplos_eventos: "",
                txt1: "Primeiro evento",
                txt2: "Segundo evento"
            }
        },
        methods: {
            primeiro(text, e){
                setTimeout(() => {
                    this.multiplos_eventos = text;
                }, 500)
            },
            segundo(text, e){
                setTimeout(() => {
                    this.multiplos_eventos = text;
                }, 1000)
            }
        }
    }
</script>

<style>
    div {
        margin: 20px;
    }
</style>