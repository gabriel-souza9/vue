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
    </div>
</template>
<script>
    export default {
        name: "Info",
        data(){
            return {
                isWorking: false,
                isShowBiel: false
            }
        }
    }
</script> 