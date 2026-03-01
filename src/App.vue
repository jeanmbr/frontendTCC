<template>
  <HeaDer />
  <PrimeiroComponente />
  <p class="paragrafo-pai">O dado de app é: {{ testando }}</p>
  <LifeCycle />
  <PessoaDados />
</template>

<script>
  import HeaDer from './components/HeaDer.vue'
  import PrimeiroComponente from './components/PrimeiroComponente.vue'
  import LifeCycle from './components/LifeCycle.vue'
  import PessoaDados from './components/PessoaDados.vue';
  export default {
    name: 'App',
    components: {
      HeaDer,
      PrimeiroComponente,
      LifeCycle,
      PessoaDados,
    }
  }
  
</script>

<style>
body{
  background-color: rgb(40,40,40);
  color: white;
}

a{
  color: turquoise;
}
  
.teste{
  background:red;
}

</style>
