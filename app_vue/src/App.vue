<template>
  <div>
    <Header />
    <PrimeiroComponent />
    <p>O dado de app é {{testando }}</p>
    <LifeCycle />
    <Pessoa />
  </div>
</template>

<script>
import PrimeiroComponent from './components/PrimeiroComponent.vue';
import LifeCycle from './components/LifeCycle.vue';
import Pessoa from './components/Pessoa.vue';
import Header from './components/Header.vue';

  export default {
    name: 'App',
    components: {
      PrimeiroComponent,
      LifeCycle,
      Pessoa,
      Header
    },
    data(){
      return {
        testando: "teste"
      }
    }
  } 
</script>

<style>
  body {
    background: #333;
    color: #eee;
  }

  a {
    color: darkcyan;
  }
</style>