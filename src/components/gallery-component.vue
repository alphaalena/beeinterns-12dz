<template>
  <div class="gallery">
      <icon-component type="image" icon-name="column"/>
      <rowComponent justify-center>
        <div class="button-dark"/>
        <div class="button-light"/>
        <div class="button-light"/>
      </rowComponent>
  </div>
</template>
<script>
import IconComponent from './icon-component'
import RowComponent from './row-component'
export default {
  name: 'galleryComponent',
  components: { RowComponent, IconComponent }
}
</script>
<style>
  .gallery {
    display: flex;
    flex-direction: column;
    width: 65%;
    padding-top: 10px;
  }
  .button-dark {
    width: 10px;
    height: 10px;
    border-radius: 50%;
    background: #000000;
    margin-right: 15px;
  }
  .button-light {
    width: 10px;
    height: 10px;
    border-radius: 50%;
    background: #D1D1D1;
    margin-right: 15px;
  }
</style>
