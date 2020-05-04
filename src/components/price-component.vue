<template>
  <p class="price">
    <slot/>
  </p>
</template>
<script>
export default {
  name: 'priceComponent'
}
</script>
<style>
  .price {
    color: #F2F2F2;
    font-size: 40px;
  }
</style>
