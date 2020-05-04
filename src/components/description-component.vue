<template>
  <div class="description">
    <slot/>
  </div>
</template>
<script>
export default {
  name: 'descriptionComponent'
}
</script>
<style>
  .description {
    width: 50%;
    text-align: left;
    padding-top: 200px;
  }
</style>
