<template>
  <div>
    <p>{{ quote }}</p>
  </div>
</template>

<script>
  export default {
    props: ['quote']
  }
</script>

<style scoped>
  div {
    border: 1px solid #ccc;
    box-shadow: 1px 1px 2px Black;
    padding: 20px;
    margin: 30px auto;
    text-align: center;
  }
</style>