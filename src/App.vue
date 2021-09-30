<template>
  <div id="app">
    <div class="container-page">
      <Header/>
      <Main/>
      <Hero/>
      <RecentSeries/>
      <SiteFeatures/>
      <Footer/>
    </div>
  </div>
</template>

<script>
import Header from './components/Header'
import Main from './components/Main'
import Hero from './components/Hero'
import RecentSeries from './components/RecentSeries'
import SiteFeatures from './components/SiteFeatures'
import Footer from './components/Footer'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Hero,
    RecentSeries,
    SiteFeatures,
    Footer
  }
}
</script>

<style lang="scss">
@import './style/common.scss';
@import './style/variables.scss';


</style>
