<template>
  <div class="container">
    <slot/>
  </div>
</template>
<script>
export default {
  name: 'containerComponent'
}
</script>
<style>
  .container {
    width: 1180px;
    margin: 0 auto;
  }
</style>
