<template>
  <p :class="type">
    <slot/>
  </p>
</template>
<script>
export default {
  name: 'descriptionTextComponent',
  props: {
    type: {
      type: String,
      default: 'text-black'
    }
  }
}
</script>
<style>
  .text-white {
    font-weight: 500;
    font-size: 16px;
    line-height: 20px;
    color: #FFFFFF;
  }
  .text-yellow {
    font-weight: 500;
    font-size: 13px;
    line-height: 20px;
    color: #FFC700;
    margin-top: 10px;
  }
  .text-black {
    font-style: normal;
    font-weight: normal;
    font-size: 16px;
    line-height: 20px;
    color: #2B2835;

  }

</style>
