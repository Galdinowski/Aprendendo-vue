<template>
  <div>
    <PrimeiroComponente />
    <p>O dado de app eh: {{ testando }}</p>
    <LifeCycle/>
    <Pessoa/>
  </div>
</template>

<script>
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from './components/Pessoa.vue'
import PrimeiroComponente from './components/PrimeiroComponente.vue'
  export default{
    name:'App',
    components:{
            PrimeiroComponente,
            LifeCycle,
            Pessoa
        }
  }
</script>