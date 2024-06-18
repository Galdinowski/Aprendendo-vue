<template>
    <div>
        <h1>Meu nome eh: {{ nome }}</h1>
    </div>


</template>

<script>
    export default{
        name: 'LifeCycle',
        data()
        {
            return {
                nome: 'Ainda nao sei'
            }
        },
        created()
        {
            setTimeout(()=>{
                this.nome = "Arthur"
            },2000)
            
        },
        mounted()
        {
            this.nome = "Lazaro"
        }

    }

</script>