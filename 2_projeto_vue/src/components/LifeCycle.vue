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
            this.lifeCycle()
            
            
        },
        mounted()
        {
            this.nome = "Lazaro"
            this.lifeCycle()
        },
        methods:{
            lifeCycle()
            {
                console.log("Executou")
            }
            
        }

    }

</script>