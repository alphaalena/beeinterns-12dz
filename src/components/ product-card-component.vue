<template>
  <div class="productCard" :style="'background-image: url(/' + card.nameImage + '.png)'">
    <column-component justify-end>
      <heading-component type="dark-bold">{{card.heading}}</heading-component>
      <p class="text">{{card.text}}</p>
      <row-component justify-start>
        <price-component color="price-bronze">{{card.price}}</price-component>
        <link-component type="frame-link-black " color="white-text">{{card.textButton}}</link-component>
      </row-component>
    </column-component>
  </div>
</template>
<script>
import HeadingComponent from './heading-component'
import PriceComponent from './price-component'
import LinkComponent from './link-component'
import ColumnComponent from './column-component'
import RowComponent from './row-component'

export default {
  name: 'productCardComponent',
  components: {
    RowComponent,
    ColumnComponent,
    LinkComponent,
    PriceComponent,
    HeadingComponent
  },
  props: {
    card: {
      type: Object
    }
  }
}
</script>
<style>
  .productCard {
    width: 393px;
    height: 560px;
    background-color: #F8F8F9;
    background-repeat: no-repeat;
    background-position: center;
    padding: 40px;
    margin-right: 37px;
  }
  .text {
    margin-bottom: 20px;
    font-weight: normal;
    font-size: 14px;
    line-height: 21px;
    color: #030303;
  }
</style>
