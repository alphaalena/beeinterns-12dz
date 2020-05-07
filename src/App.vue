<template>
  <div id="app">
    <header-component>
      <container-component>
        <row-component>
          <logo-component/>
          <linkComponent class="padding-top" type="link" color="white-text" :key="link" v-for="link in links">{{link}}
          </linkComponent>
          <div v-for="icon in icons" :key="icon" class="padding-top">
            <icon-component :icon-name="icon" v-if="icon" type="icon"/>
          </div>
        </row-component>
      </container-component>
    </header-component>
    <main-component>
      <column-component>
        <section-component type="section-dark">
          <container-component>
            <row-component>
              <headphones-background-component/>
              <description-component>
                <description-text-component type="text-white">Beats Studio3 Wireless</description-text-component>
                <heading-component type="light">
                  Experience your <br> music like never before.
                </heading-component>
                <row-component justify-start>
                  <price-component color="price-light">$299.95</price-component>
                  <link-component type="frame-link-yellow" color="black-text">buy now</link-component>
                </row-component>
                <description-text-component type="text-yellow">$60 Apple Music gift card with purchase of select Beats
                  products.*
                </description-text-component>
              </description-component>
            </row-component>
          </container-component>
        </section-component>
        <section-component type="section-light">
          <container-component>
            <row-component>
              <description-component>
                <description-text-component type="text-black">Portable Wireless Speaker</description-text-component>
                <heading-component type="dark-bold">Beats Pill<sup>+</sup></heading-component>
                <heading-component type="dark">Available Colors</heading-component>
                <description-text-component type="text-black">Find your Color</description-text-component>
                <row-component justify-start>
                  <div class="margin" :key="color" v-for="color in colors">
                    <color-picker-component v-if="color" :color="color"/>
                  </div>
                </row-component>
                <row-component justify-start>
                  <price-component color="price-dark">$299.95</price-component>
                  <link-component type="frame-link-black " color="white-text">buy now</link-component>
                </row-component>
                <description-text-component type="text-black-little">$60 Apple Music gift card with purchase of select
                  Beats products.*
                </description-text-component>
              </description-component>
              <gallery-component/>
            </row-component>
          </container-component>
        </section-component>
        <section-component type="section-light">
          <container-component>
            <row-component>
              <product-card-component :key="card.nameImage" v-for="card in cards" :card="card"/>
            </row-component>
          </container-component>
        </section-component>
      </column-component>
    </main-component>
    <footer-component>
      <container-component>
        <column-component>
          <row-component>
            <logo-component/>
            <column-component>
              <heading-component type="whites">Products</heading-component>
              <link-component type="link" color="white-text-min" :key="product" v-for="product in products">{{product}}
              </link-component>
            </column-component>
            <column-component>
              <heading-component type="whites">Support</heading-component>
              <link-component type="link" color="white-text-min" :key="support" v-for="support in supports">{{support}}
              </link-component>
            </column-component>
            <column-component>
              <heading-component type="whites">Company</heading-component>
              <link-component type="link" color="white-text-min" :key="company" v-for="company in companies">{{company}}
              </link-component>
            </column-component>
            <column-component>
              <heading-component type="whites">Follow us</heading-component>
              <row-component justify-start>
                <div :key="net" v-for="net in nets">
                  <icon-component :icon-name="net" v-if="net" type="icon"/>
                </div>
              </row-component>
            </column-component>
          </row-component>
          <description-text-component type="text-white-little">Copyright © 2020 Apple Inc. - All rights reserved.
          </description-text-component>
        </column-component>
      </container-component>
    </footer-component>
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
import ColorPickerComponent from './components/color-picker -component'
import GalleryComponent from './components/gallery-component'
import ProductCardComponent from './components/ product-card-component'
import FooterComponent from './components/footer-component'
export default {
  name: 'App',
  components: {
    FooterComponent,
    ProductCardComponent,
    GalleryComponent,
    ColorPickerComponent,
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
      icons: ['search', 'basket', 'lk'],
      colors: ['white', 'red', 'black'],
      cards: [
        {
          nameImage: 'earphone1',
          heading: 'Beatsˣ',
          text: 'Up to 8 hours of battery life\n' +
              'With Fast Fuel, a 5-minute charge = 2 hours of playback',
          price: '$999.95',
          textButton: 'buy now'
        },
        {
          nameImage: 'earphone3',
          heading: 'Beatsˣ',
          text: 'Up to 8 hours of battery life\n' +
              'With Fast Fuel, a 5-minute charge = 2 hours of playback',
          price: '$99.95',
          textButton: 'buy now'
        },
        {
          nameImage: 'earphone2',
          text: 'Up to 8 hours of battery life\n' +
              'With Fast Fuel, a 5-minute charge = 2 hours of playback',
          price: '$299.95',
          textButton: 'buy now'
        }],
      products: ['headphones', 'earpphones', 'speakers', 'accessories', 'collaborations', 'beatsaudio', 'special offers'],
      supports: ['product help', 'service & warranty', 'register your beats', 'update your beats', 'authorized service providers', 'contact support', 'international numbers'],
      companies: ['product help', 'news and events', 'promotion terms', 'privacy policy', 'trademark', 'terms of use', 'cookies'],
      nets: ['insta', 'fb', 'tw', 'whatsapp']
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
