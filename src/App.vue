<template>
  <div id="app">
    <experiment1></experiment1>
    <experiment2></experiment2>
  </div>
</template>

<script>
import Experiment1 from './components/parent-to-children/Experiment1'
import Experiment2 from './components/children-to-parent/Experiment2'

export default {
  name: 'app',
  components: {
    'experiment1': Experiment1,
    'experiment2': Experiment2
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
