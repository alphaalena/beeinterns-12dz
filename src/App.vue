<template>
  <div id="app">
    <header-component>
      <row-component>
        <logo-component/>
        <linkComponent  class="padding-top"  type="link" color="white-text" :key="link" v-for="link in links">{{link}}</linkComponent>
        <div v-for="icon in icons" :key="icon" class="padding-top" >
          <icon-component :icon-name="icon" v-if="icon"/>
        </div>
      </row-component>
    </header-component>
    <main-component>
      <column-component>
        <section-component type="section-dark">
          <row-component>
            <headphones-background-component/>
            <description-component>
                  <description-text-component type="text-white" >Beats Studio3 Wireless </description-text-component>
                  <heading-component type="light">
                    Experience your <br> music like never before.
                  </heading-component>
                <container-component>
                <price-component>$299.95</price-component>
                  <link-component type="frame-link" color="black-text">buy now</link-component>
                </container-component>
                <description-text-component type="text-yellow">$60 Apple Music gift card with purchase of select Beats products.*</description-text-component>
            </description-component>
          </row-component>
        </section-component>
        <section-component type="section-light">
          <row-component>
            <description-component>
              <description-text-component type="text-black">Portable Wireless Speaker</description-text-component>
              <heading-component type="dark-bold">Beats Pill<sup>+</sup></heading-component>
              <heading-component type="dark">Available Colors</heading-component>
              <description-text-component type="text-black">Find your Color</description-text-component>
            </description-component>
          </row-component>
        </section-component>
      </column-component>
    </main-component>
  </div>
</template>

<script>
import HeaderComponent from './components/header-component'
import RowComponent from './components/row-component'
import LogoComponent from './components/logo-component'
import LinkComponent from './components/link-component'
import IconComponent from './components/icon-component'
import MainComponent from './components/main-component'
import ColumnComponent from './components/column-component'
import SectionComponent from './components/section-component'
import HeadphonesBackgroundComponent from './components/headphones-background-component'
import DescriptionComponent from './components/description-component'
import DescriptionTextComponent from './components/description-text-component'
import HeadingComponent from './components/heading-component'
import PriceComponent from './components/price-component'
import ContainerComponent from './components/container-component'
export default {
  name: 'App',
  components: {
    ContainerComponent,
    PriceComponent,
    HeadingComponent,
    DescriptionTextComponent,
    DescriptionComponent,
    HeadphonesBackgroundComponent,
    SectionComponent,
    ColumnComponent,
    MainComponent,
    IconComponent,
    LinkComponent,
    LogoComponent,
    RowComponent,
    HeaderComponent
  },
  data () {
    return {
      links: ['headphones', 'earphones', 'speakers', 'explore'],
      icons: ['search', 'basket', 'lk']
    }
  }
}
</script>

<style>
#app {
  font-family: 'Open Sans', serif;
  text-align: center;
}
</style>
