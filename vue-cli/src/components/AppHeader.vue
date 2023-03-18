<template>
  <div>
    <header><h1>{{ propsdata }}</h1></header>
    <button v-on:click="sendEvent">send</button>
  </div>
</template>

<script>
export default {
  props:['propsdata'],
  methods: {
    sendEvent: function() {
      this.$emit('renew');
    }
  }
}
</script>

<style>

</style>