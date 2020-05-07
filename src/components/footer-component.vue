<template>
  <footer class="footer">
    <slot/>
  </footer>
</template>
<script>
export default {
  name: 'footerComponent'
}
</script>
<style>
  .footer {
    height: 360px;
    background-color: #2B2835;
    padding-top: 40px;
  }
</style>
