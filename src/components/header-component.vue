<template>
  <header class="header">
    <slot/>
  </header>
</template>
<script>
export default {
  name: 'headerComponent'
}
</script>
<style>
  .header{
    position: fixed;
    left: 0;
    right: 0;
    height: 78px ;
    background: rgba(25, 23, 32, 0.47);
    z-index: 1;
  }
</style>
