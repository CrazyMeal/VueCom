<template>
  <div id="app">
    <experiment1></experiment1>
  </div>
</template>

<script>
import Experiment1 from './components/Experiment1'

export default {
  name: 'app',
  components: {
    'experiment1': Experiment1
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}


</style>
