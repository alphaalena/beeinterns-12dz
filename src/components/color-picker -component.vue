<template>
  <div :class="color">
  </div>
</template>
<script>
export default {
  name: 'colorPickerComponent ',
  props: {
    color: {
      type: String,
      default: 'white'
    }
  }
}
</script>
<style>
  .white {
    width: 37px;
    height: 37px;
    background-color: #FFFFFF;
    border: 1px solid #EAEAEA;
    border-radius: 50%;
  }
  .red {
    width: 37px;
    height: 37px;
    background-color: #DD5656;
    border: 1px solid #EAEAEA;
    border-radius: 50%;
  }
  .black {
    width: 37px;
    height: 37px;
    background-color: #000000;
    border: 1px solid #EAEAEA;
    border-radius: 50%;
  }
</style>
