<template>
  <section :class="type">
    <slot/>
  </section>
</template>
<script>
export default {
  name: 'sectionComponent',
  props: {
    type: {
      type: String,
      default: 'section-dark'
    }
  }
}
</script>
<style>
  .section-dark {
    width: 100%;
    height: 766px;
    margin: 0 auto;
    background: linear-gradient( #2B2835 80% , #FBFCFF 20% );
  }
  .section-light {
    width: 100%;
    margin: 0 auto;
    background-color: #FBFCFF;
    padding-bottom: 70px;
  }

</style>
