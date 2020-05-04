<template>
  <div id="app">
    <header-component>
      <row-component>
        <logo-component/>
        <LinkComponent  class="padding-top" :key="link" v-for="link in links">{{link}}</LinkComponent>
        <div v-for="icon in icons" :key="icon" class="padding-top" >
          <icon-component :icon-name="icon" v-if="icon"/>
        </div>
      </row-component>
    </header-component>
    <main-component>
      <column-component>
        <section-component>
          <row-component>
            <headphones-background-component/>
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
export default {
  name: 'App',
  components: {
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
