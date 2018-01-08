<template>
  <div id="app">
    <app-quote>
      <h2 slot="title">{{ quoteTitle }}</h2>
      <p slot="content">A Wonderful Quote!</p>
    </app-quote>
  </div>
</template>

<script>
  import Quote from './components/Quote.vue';

  export default {
    data: function () {
      return {
        quoteTitle: 'A Great Quote'
      }
    },
    components: {
      appQuote: Quote
    }
  }
</script>

<style lang="scss">

</style>
