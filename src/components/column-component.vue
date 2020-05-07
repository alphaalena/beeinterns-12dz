<template>
  <div class="column" :justify-end="justifyEnd">
    <slot/>
  </div>
</template>
<script>
export default {
  name: 'columnComponent',
  props: {
    justifyEnd: Boolean
  }
}
</script>
<style>
  .column {
    display: flex;
    flex-direction: column;
  }
  .column[justify-end] {
    height: 100%;
    justify-content: flex-end;
    text-align: left;
  }
</style>
