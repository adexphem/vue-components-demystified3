<template>
  <div id="app">
    <app-quote>
      <h2>The Quote</h2>
      <p>A Wonderful Quote!</p>
    </app-quote>
  </div>
</template>

<script>
  import Quote from './components/Quote.vue';

  export default {
    components: {
      appQuote: Quote
    }
  }
</script>

<style lang="scss">

</style>
