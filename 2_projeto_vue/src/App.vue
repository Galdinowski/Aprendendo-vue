<template>
  <div>
    <Header/>
    <PrimeiroComponente />
    <p>O dado de app eh: {{ testando }}</p>
    <LifeCycle/>
    <Pessoa/> 

  </div>
</template>

<script>
import Header from './components/Header.vue'
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from './components/Pessoa.vue'
import PrimeiroComponente from './components/PrimeiroComponente.vue'
  export default{
    name:'App',
    components:{
            PrimeiroComponente,
            LifeCycle,
            Pessoa,
            Header,
            
        },

  }
</script>

<style>
  body{
    background-color: rgb(26, 92, 97);
  }

</style>