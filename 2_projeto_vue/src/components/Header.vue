<template>
    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Projetos</a></li>
        <li><a href="#">Contatos</a></li>

    </ul>

</template>

<script>
    export default{
        name: 'Header'

    }

</script>

<style scoped>
    ul{
        list-style: none;
        display: flex;
        background-color: beige;
    }

    li{
        margin-right: 10px;
    }

    a{
        color:rgb(233, 132, 0);
        text-decoration: none;
        transition: 1s;
        
    }
    a:hover{
        color: blue;
    }

</style>