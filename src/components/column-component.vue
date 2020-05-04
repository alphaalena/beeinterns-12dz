<template>
  <div class="column">
    <slot/>
  </div>
</template>
<script>
export default {
  name: 'columnComponent'
}
</script>
<style>
  .column {
    display: flex;
    flex-direction: column;
  }
</style>
