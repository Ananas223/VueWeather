<template>
  <InformerContainer v-bind:weather="weather"/>
</template>

<script>
import InformerContainer from './components/Container.vue'

export default {
  name: 'App',
  components: {
    InformerContainer
  },
  data(){
    return{
      weather: {
        real: '1',
        feel: '-3,2',
        humidity: '6',
        wind: 20
      }
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
