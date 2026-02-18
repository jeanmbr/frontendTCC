<template>
  <PrimeiroComponente />
  <LifeCycle />
  <PessoaDados />
</template>

<script>

  import PrimeiroComponente from './components/PrimeiroComponente.vue'
  import LifeCycle from './components/LifeCycle.vue'
  import PessoaDados from './components/PessoaDados.vue';
  export default {
    name: 'App',
    components: {
      PrimeiroComponente,
      LifeCycle,
      PessoaDados,
    }
  }
  
</script>
