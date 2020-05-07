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
  .white-text {
    padding: 12px 45px;
    color: #FFFFFF;
    font-size: 15px;
    text-transform: uppercase;
  }
  .white-text-min {
    text-align: left;
    color: #FFFFFF;
    font-size: 14px;
    line-height: 31px;
    font-weight: 200;
    text-transform: uppercase;
  }
  .link {
    text-decoration: none;
  }
  .frame-link-yellow {
    text-decoration: none;
    width: 170px;
    height: 41px;
    background: #FFC700;
    border-radius: 100px ;
    margin-left: 35px;
  }
  .black-text {
    padding: 12px 45px;
    font-weight: 600;
    font-size: 14px;
    text-transform: uppercase;
    color: #000000;
  }
  .frame-link-black {
    text-decoration: none;
    width: 170px;
    height: 41px;
    background: #000000;
    border-radius: 100px ;
    margin-left: 43px;
  }

</style>
