<template>
    <ul>
        <li>
            <a href="#">Home</a>
        </li>
        <li>
            <a href="#">Projetos</a>
        </li>
        <li>
            <a href="#">Contato</a>
        </li>
    </ul>
    
</template>
<script>
    export default {
        name: 'Header'
    }
</script>

<style scoped>

    ul {
        list-style: none;
        display: flex;
        background: rgb(6, 54, 187);
    }

    li {
        margin-right: 10px;
    }

    a {
        color: #ddd;
        text-decoration: none;
        transition: .5s;
    }

    a:hover {
        color: rgb(60, 216, 200);
    }


</style>