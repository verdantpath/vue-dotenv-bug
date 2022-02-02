<template>
  <div id="app">
    <h2> Hello world!</h2>
    <p>NODE_ENV: {{ nodeEnvTest }}</p>
  </div><!-- / #app -->
</template>

<script>

export default {
  name: 'app',
  data () {
    return {
      nodeEnvTest: process.env.NODE_ENV
    }
  },
  created() {
    console.log(process.env.NODE_ENV);
  }
}

</script>

<style lang="scss">

</style>