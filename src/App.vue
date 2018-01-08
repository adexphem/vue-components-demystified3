<template>
  <div id="app">
    <app-quote quote="A wonderful quote!"></app-quote>
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
