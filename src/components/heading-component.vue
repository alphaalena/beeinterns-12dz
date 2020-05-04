<template>
  <h1 :class="type">
    <slot/>
  </h1>
</template>
<script>
export default {
  name: 'headingComponent',
  props: {
    type: {
      type: String,
      default: 'light'
    }
  }
}
</script>
<style>
  .light {
    font-size: 40px;
    color: #FBFCFF;
  }
  .dark-bold {
     font-weight: bold;
     font-size: 50px;
     line-height: 55px;
     color: #2B2835;
   }
  .dark {
    font-size: 40px;
    line-height: 55px;
    color: #2B2835;
  }
</style>
