<template>
  <div id="app">
    <Header/>
    <Hero :bgImg="require('./assets/images/jumbotron.jpg')"/>
    <Content/>
    <MegaIcons/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import Content from './components/Content.vue'
import MegaIcons from './components/MegaIcons.vue'
import Footer from './components/Footer.vue'


export default {
  name: 'App',
  components: {
    Header,
    Hero,
    Content,
    MegaIcons,
    Footer
  }
}
</script>

<style lang="scss">
@import './assets/style/common.scss';
</style>
