<template>
    <div>
       <h2>
            Meu Formulário
       </h2> 

       <form @submit="submit($event)">
            <div>
                <input type="text" v-model="name">
            </div>
            <div>
                <input type="text" v-model="email">
            </div>

            <div>
                <input type="submit" value="Enviar">
            </div>

       </form>
    </div>
</template>

<script>
    export default {
        name: "Form",
        methods: {
            submit(e){
                e.preventDefault();
                console.log(this.name, this.email)
            }
        },
        data(){
            return {
                name: "",
                email: ""
            }
        }
        
    }

</script>