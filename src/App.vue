<template>
  <div id="app">
    <Header/>
    <Main/>
    <Footer/>
    <Ancora/>
    <SideTags/>
  </div>
</template>

<script>
import Header from './components/macro/Header.vue'
import Main from './components/macro/Main.vue'
import Footer from './components/macro/Footer.vue'
import Ancora from './components/elements/Ancora.vue'
import SideTags from './components/elements/SideTags.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
    Ancora,
    SideTags
  }
}
</script>

<style lang="scss">
@import './assets/style/global.scss';

</style>
