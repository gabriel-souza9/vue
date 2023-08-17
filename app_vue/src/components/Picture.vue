<template>
    <div>
        <img :src="avatar2" :alt="description" style="height: 240px; margin-top: 20px;" >
        <MudarAvatar @mudar-imagem="trocarImg" />
    </div>
</template>

<script>
import MudarAvatar from './MudarAvatar.vue';
    export default {
        name: "Picture",
        components: {
            MudarAvatar
        },
        methods: {
            trocarImg(){
                console.log("teste")
                this.avatar2 = this.avatar
            }
        },  
        data(){
            return {
                avatar: "https://avatars.githubusercontent.com/u/82981798?v=4",
                avatar2: "https://s2-ge.glbimg.com/uURVDi5PyzxnFsHYLQ_99mtKrGc=/187x110:788x745/984x0/smart/filters:strip_icc()/i.s3.glbimg.com/v1/AUTH_bc8228b6673f488aa253bbcb03c80ec5/internal_photos/bs/2023/1/X/g9YBnzSzmhM60cvB5GSg/raposao.jpg",
                description: "Souzinha png"
            }
        }
    }
</script>