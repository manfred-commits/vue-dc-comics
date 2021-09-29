<template>
  <div id="app">
    <div class="container-page">
      <Header/>
      <Main/>
      <Footer/>
    </div>
  </div>
</template>

<script>
import Header from './components/Header'
import Main from './components/Main'
import Footer from './components/Footer'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
@import './style/common.scss';
@import './style/variables.scss';


</style>
