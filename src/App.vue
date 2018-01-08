<template>
  <div id="app">
    <p>
      <button @click="dynamicComponent = 'appAuthor'">Author</button>
      <button @click="dynamicComponent = 'appNew'">New</button>
      <button @click="dynamicComponent = 'appQuote'">Quote</button>
    </p>

    <hr>

    <p>{{ dynamicComponent }}</p>

    <!--using keep-alive to retain the state of a component-->
    <keep-alive>
      <component :is="dynamicComponent">Default Content</component>
    </keep-alive>
  </div>
</template>

<script>
  import New from './components/New.vue';
  import Author from './components/Author.vue';
  import Quote from './components/Quote.vue';

  export default {
    data: function () {
      return {
        quoteTitle: 'A Great Quote',
        dynamicComponent: 'appQuote'
      }
    },
    components: {
      appQuote: Quote,
      appAuthor: Author,
      appNew: New
    }
  }
</script>

<style lang="scss">

</style>
