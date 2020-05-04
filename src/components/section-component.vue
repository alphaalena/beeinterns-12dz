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
    height: 618px;
    margin: 0 auto;
    background-color: #2B2835;
  }

</style>
