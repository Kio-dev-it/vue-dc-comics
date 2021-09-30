<template>
  <div id="app">
    <Header/>
    <Content/>
    <MegaIcon/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Content from './components/Content.vue'
import MegaIcon from './components/MegaIcon.vue'
import Footer from './components/Footer.vue'


export default {
  name: 'App',
  components: {
    Header,
    Content,
    MegaIcon,
    Footer
  }
}
</script>

<style lang="scss">
</style>
