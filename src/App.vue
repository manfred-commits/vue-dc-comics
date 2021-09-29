<template>
  <div id="app">
    <div class="container-page">
      <Header/>
      <Main/>
      <SiteFeatures/>
      <Footer/>
    </div>
  </div>
</template>

<script>
import Header from './components/Header'
import Main from './components/Main'
import SiteFeatures from './components/SiteFeatures'
import Footer from './components/Footer'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    SiteFeatures,
    Footer
  }
}
</script>

<style lang="scss">
@import './style/common.scss';
@import './style/variables.scss';


</style>
