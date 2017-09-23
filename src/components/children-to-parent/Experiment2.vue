<template>
  
  <div id="experiment2">
    <h4>Second Experimentation</h4>
    <h5>Communication from children to parent</h5>
    <p>
      Last value to received from children: <span style="color:red">{{ message }}</span>
      <div>
        <children2 v-on:sendingToParentEvent="updateValueReceived($event)"></children2>
      </div>
    </p>
  </div>
</template>

<script>

import Children2 from './Children2'

export default {
  name: 'Experiment2',
  data () {
    return {
      message: ''
    }
  },
  methods: {
    updateValueReceived: function (messageReceived) {
      console.log(messageReceived)
      this.message = messageReceived
    }
  },
  components: {
    'children2': Children2
  }
}
</script>

<style>
#experiment2 {
  float: left;
  width: 50%;
  border-style: dashed;
  margin-top: 10px;
  padding-left: 10px;
  padding-bottom: 10px;
}
</style>