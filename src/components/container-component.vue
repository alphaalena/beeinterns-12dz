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
    display: flex;
    flex-direction: row;
  }
</style>
