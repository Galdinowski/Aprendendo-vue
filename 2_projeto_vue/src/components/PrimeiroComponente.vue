<template>
    <div>
        <h1>Ola vue</h1>
        <p>Meu nome eh: {{ name }}</p>
    </div>
    
</template>

<script>
    export default{
    
        name:'PrimeiroComponente',
        data()
        {
            return {
                name: "Arthur"
            }
        }
        
    }
</script>