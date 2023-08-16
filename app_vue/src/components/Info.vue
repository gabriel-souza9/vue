<template>
    <div>
        <p v-if="isWorking">Estou trabalhando no momento.</p>
        <p v-else>Estou em busca de novas oportunidade</p>
        <p>utilizo as seguintes tecnologias:</p>
        <ul>
            <li>Javascript</li>
            <li>Node</li>
            <li>React</li>
        </ul>
        <p v-show="isShowBiel">bielzin lindin</p>
        <p>Para acessar meu portfólio <a  v-bind:href="myLink">basta clicar aqui</a></p>
        
        <Picture />    

    </div>
</template>

<script>
import Picture from './Picture.vue'
    export default {
        name: "Info",
        components: {
            Picture
        },
        data(){
            return {
                isWorking: false,
                isShowBiel: false,
                myLink: "https://google.com"
            }
        }
    }
</script> 