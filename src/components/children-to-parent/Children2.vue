<template>
  <div id="children2">
    <p>
      Value to send to parent: <input type="text" v-model="message"><button v-on:click="sendToParent">Send value</button>
    </p>
  </div>
</template>

<script>

export default {
  name: 'Children2',
  data () {
    return {
      message: ''
    }
  },
  methods: {
    sendToParent: function () {
      this.$emit('sendingToParentEvent', this.message)
    }
  },
  components: {
  }
}
</script>

<style>
#children2 {
  float: left;
  width: 90%;
  border-style: dotted;
  margin-top: 10px;
  margin-left: 10px;
}
</style>