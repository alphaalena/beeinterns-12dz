<template>
  <div class="row">
    <slot/>
  </div>
</template>
<script>
export default {
  name: 'rowComponent'
}
</script>
<style>
  .row {
    margin: 0 auto;
    justify-content: space-between;
    text-align: center;
    display: flex;
    flex-direction: row;
    width: 1180px;
  }
</style>
