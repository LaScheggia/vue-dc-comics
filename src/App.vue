<template>
  <div id="app">
    <header-comp/>
    <hero-banner-comp/>
    <main-comp/>
    <jumbo-comp/>
    <footer-comp/>


  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue'
import HeroBannerComp from './components/HeroBannerComp.vue'
import MainComp from './components/MainComp.vue'
import JumboComp from './components/JumboComp.vue'
import FooterComp from './components/FooterComp.vue'


export default {
  name: 'App',
  components: {
    HeaderComp,
    HeroBannerComp,
    MainComp,
    JumboComp,
    FooterComp,
  }
}
</script>


<style lang="scss">
@import './assets/style/general.scss';
@import './assets/style/utilities.scss'

</style>
