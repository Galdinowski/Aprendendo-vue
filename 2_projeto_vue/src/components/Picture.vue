<template>
    <img :src="avatar" :alt="descricao">
</template>

<script>
    export default{
        name: 'Pictures',
        data()
        {
            return{
                avatar: "/img/avatar.png",
                descricao: "Arthur Galdino"
            }
        }
    }
</script>