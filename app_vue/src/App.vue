<template>
  <div>
    <PrimeiroComponent />
    <p>O dado de app é {{ testando }}</p>
  </div>
</template>

<script>
import PrimeiroComponent from './components/PrimeiroComponent.vue';
  export default {
    name: 'App',
    components: {
      PrimeiroComponent
    },
    data(){
      return {
        testando: "teste"
      }
    }
  }
</script>