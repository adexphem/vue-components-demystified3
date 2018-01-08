<template>
  <div>
    <div class="title">
      <slot name="title"></slot>
      <span class="subtitle"><slot name="subtitle">Default Title</slot></span>
    </div>
    <div class="content">
      <slot name="content"></slot>
    </div>
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

  h2 {
    color: #f9cd0b;
  }

  .title {
    font-style: italic;
  }

  .content {
    font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  }

  .subtitle {
    color: #ccc;
  }
</style>