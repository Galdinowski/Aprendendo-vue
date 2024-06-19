<template>
    <div>
        <h2>Esta eh a descricao da pessoa : {{ nome }} </h2>
        <Info/>
        <Formu/>
    </div>    

</template>

<script>
    import Info from './Info.vue'
    import Formu from './Form.vue'
    export default{
        name: 'Pessoa',
        components:{
            Info,Formu
        },
        data()
        {
            return {
                nome: "Tutubarao"
            }
        }
    }
</script>