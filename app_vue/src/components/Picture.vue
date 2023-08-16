<template>
    <img :src="avatar" :alt="description" style="height: 240px; margin-top: 20px;" >
</template>

<script>
    export default {
        name: "Picture",
        data(){
            return {
                avatar: "https://avatars.githubusercontent.com/u/82981798?v=4",
                description: "Souzinha png"
            }
        }
    }
</script>