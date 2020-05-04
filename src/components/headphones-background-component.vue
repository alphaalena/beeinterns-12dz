<template>
  <div class="background">
    <slot/>
  </div>
</template>
<script>
export default {
  name: 'headphonesBackgroundComponent'
}
</script>
<style>
  .background {
    width: 866px;
    height: 766px;
    background-image: url("../assets/Bitmap.png") ;
    background-repeat: no-repeat;
    transform: translateX(-85px);
  }

</style>
