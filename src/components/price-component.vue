<template>
  <p :class="color">
    <slot/>
  </p>
</template>
<script>
export default {
  name: 'priceComponent',
  props: {
    color: {
      type: String,
      default: 'price-dark'
    }
  }
}
</script>
<style>
  .price-light {
    color: #F2F2F2;
    font-size: 40px;
  }
  .price-dark {
    font-size: 40px;
    color: #000000;
  }
  .price-bronze {
    font-weight: 600;
    font-size: 25px;
    line-height: 30px;
    color: #9D8220;

  }
</style>
