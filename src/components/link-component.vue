<template>
  <a href="#" :class="type"><p :class="color"><slot/></p></a>
</template>
<script>
export default {
  name: 'linkComponent',
  props: {
    type: {
      type: String,
      default: 'link'
    },
    color: {
      type: String,
      default: 'white-text'
    }
  }
}
</script>
<style>
  .white-text{
    color: #FFFFFF;
    font-size: 15px;
    text-transform: uppercase;
    padding-right: 20px;
  }
  .link {
    text-decoration: none;
  }
  .frame-link {
    text-decoration: none;
    width: 170px;
    height: 41px;
    background: #FFC700;
    border-radius: 100px ;
    margin-left: 35px;
  }
  .black-text {
    padding: 10px 45px;
    font-weight: 600;
    font-size: 14px;
    text-transform: uppercase;
    color: #000000;
  }

</style>
