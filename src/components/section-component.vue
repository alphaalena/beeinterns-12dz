<template>
  <section class="section">
    <slot/>
  </section>
</template>
<script>
export default {
  name: 'sectionComponent'
}
</script>
<style>
  .section {
    width: 100%;
    height: 766px;
    margin: 0 auto;
    background: linear-gradient( #2B2835 80% , #FBFCFF 20% );
  }

</style>
