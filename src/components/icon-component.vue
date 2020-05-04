<template>
  <img class="icon" :src="'/' + iconName + '.png'">
</template>
<script>
export default {
  name: 'iconComponent',
  props: {
    iconName: {
      type: String,
      required: true
    }
  }
}
</script>
<style>
  .icon{
    width: 27px ;
    height: 27px;
    margin-right: 20px;
  }
</style>
