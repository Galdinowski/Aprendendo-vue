<template>
    <div>
        <h1>Ola vue</h1>
        <p>Meu nome eh: {{ name }}</p>
        <MultiplosEventos/>
    </div>
    
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue';

    export default{
    
        name:'PrimeiroComponente',
        components: {

                MultiplosEventos

        },

        data()
        {
            return {
                name: "Arthur"
            }
        }
        
    }
</script>