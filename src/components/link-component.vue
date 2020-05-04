<template>
  <a href="#" class="link"><p class="link-view"><slot/></p></a>
</template>
<script>
export default {
  name: 'linkComponent'
}
</script>
<style>
  .link-view {
    color: #FFFFFF;
    font-size: 15px;
    text-transform: uppercase;
    padding-right: 20px;
  }
  .link {
    text-decoration: none;
  }

</style>
