<template>
  <div id="children1">
    <p>
      I'm a child and my parent tell me: <span style="color:red">{{ messageReceived }}</span>
    </p>
  </div>
</template>

<script>

export default {
  name: 'Children1',
  props: ['messageReceived'],
  data () {
    return {
    }
  },
  components: {
  }
}
</script>

<style>
#children1 {
  float: left;
  width: 40%;
  border-style: dotted;
  margin-top: 10px;
  margin-left: 10px;
}
</style>