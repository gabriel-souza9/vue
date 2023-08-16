<template>
    <div>
        <p v-if="isWorking">Estou trabalhando no momento.</p>
        <p v-else>Estou em busca de novas oportunidade</p>
        <h3>Tecnologias de Back que eu utilizo:</h3>
        <ul >
            <li v-for="(tech, i) in backTechs" :key="i">
                {{ tech }}
            </li>
        </ul>

        <h3>Tecnologias de Front que eu utilizo:</h3>
        <ul >
            <li v-for="tech in frontTechs" :key="tech.id">
                {{ tech.langue }}
            </li>
        </ul>

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
                myLink: "https://github.com/gabrielp1999/",
                backTechs: ["Javascript", "Python", "Node"],
                frontTechs: [
                    { id: 1, langue: "HTML" },
                    { id: 1, langue: "CSS" },
                    { id: 1, langue: "Vue" }
                ]
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