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
    margin-top: 13px;
    font-weight: bold;
  }
  .dark-bold {
     font-weight: bold;
     font-size: 50px;
     line-height: 55px;
     color: #2B2835;
     margin-top: 7px;
    margin-bottom: 5px;
   }
  .dark {
    font-size: 40px;
    line-height: 55px;
    color: #2B2835;
    margin-top: 20px;
    margin-bottom: 10px;
  }
  .whites {
    font-size: 24px;
    font-weight: bold;
    color: #FFFFFF;
    text-align: left;
    margin-top: 10px;
  }
</style>
