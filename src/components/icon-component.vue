<template>
    <img :class="type" :src="'/' + iconName + '.png'" >
</template>
<script>
export default {
  name: 'iconComponent',
  props: {
    iconName: {
      type: String,
      required: true
    },
    type: {
      type: String,
      required: 'icon'
    }
  }
}
</script>
<style>
  .icon {
    width: 33px ;
    height: 30px;
    margin-right: 10px;
    margin-top: 5px;
  }
  .image  {
  }
</style>
