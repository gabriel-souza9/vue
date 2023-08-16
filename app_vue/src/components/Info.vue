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
        <p v-show="isShowBiel">bielzin</p>
        <p>Para acessar meu portfólio <a  v-bind:href="myLink">basta clicar aqui</a></p>

        <button @click="showPicture()">
           {{ textBtnPicture }}
        </button>

        <div>
            <Picture v-show="isShowBiel"/>    
        </div>
        

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
                textBtnPicture: "Mostrar Imagem",
                myLink: "https://google.com"
            }
        },
        methods: {
            showPicture(){
                this.isShowBiel = !this.isShowBiel
                if(!this.isShowBiel){
                    this.textBtnPicture = "Mostrar Imagem";
                }else {
                    this.textBtnPicture = "Fechar Imagem";
                }
            }
        }

    }
</script> 