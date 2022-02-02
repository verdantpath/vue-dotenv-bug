<template>
  <div id="app">
    <h2> Hello world!</h2>
    <p>NODE_ENV: {{ nodeEnvTest }}</p>
    <p>BASE_URL: {{ baseUrlTest }}</p>
    <p>VUE_APP_TEST: {{ dotEnvFileTest }}</p>
  </div><!-- / #app -->
</template>

<script>

export default {
  name: 'app',
  data () {
    return {
      nodeEnvTest: process.env.NODE_ENV,
      baseUrlTest: process.env.BASE_URL,
      dotEnvFileTest: process.env.VUE_APP_TEST
    }
  },
  created() {
    console.log("process.env.NODE_ENV", process.env.NODE_ENV);
    console.log("process.env.BASE_URL", process.env.BASE_URL);
    console.log("process.env.VUE_APP_TEST", process.env.VUE_APP_TEST);
  }
}

</script>

<style lang="scss">

</style>