<template>
  
  <div id="experiment1">
    <h4>First Experimentation</h4>
    <h5>Communication from parent to children</h5>
    <p>
      Value to send to children: <input type="text" v-model="message">
      <div>
        <children1 v-bind:messageReceived="message"></children1>
        <children1 v-bind:messageReceived="message"></children1>
      </div>
    </p>
  </div>
</template>

<script>

import Children1 from './Children1'

export default {
  name: 'Experiment1',
  data () {
    return {
      message: ''
    }
  },
  components: {
    'children1': Children1
  }
}
</script>

<style>
#experiment1 {
  float: left;
  width: 50%;
  border-style: dashed;
  padding-left: 10px;
  padding-bottom: 10px;
}
</style>