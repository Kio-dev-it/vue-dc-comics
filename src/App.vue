<template>
  <div id="app">
    <Header/>
    <Content/>
    <MegaIcons/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Content from './components/Content.vue'
import MegaIcons from './components/MegaIcons.vue'
import Footer from './components/Footer.vue'


export default {
  name: 'App',
  components: {
    Header,
    Content,
    MegaIcons,
    Footer
  }
}
</script>

<style lang="scss">
@import './assets/style/common.scss';
</style>
