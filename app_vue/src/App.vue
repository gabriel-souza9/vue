<template>
  <div>
    <PrimeiroComponent />
    <p>O dado de app é {{testando }}</p>
    <LifeCycle />
  </div>
</template>

<script>
import PrimeiroComponent from './components/PrimeiroComponent.vue';
import LifeCycle from './components/LifeCycle.vue';

  export default {
    name: 'App',
    components: {
      PrimeiroComponent,
      LifeCycle
    },
    data(){
      return {
        testando: "teste"
      }
    }
  } 
</script>