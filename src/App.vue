<template>
  <div id="app">
    
    <Header/>

    <main>
      <Hero :imgBg="require('./assets/img/jumbotron.jpg')"/>
      <Comics/>
    </main>

    <Footer/>

  </div>
</template>

<script>
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import Comics from './components/Comics.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Hero,
    Comics,
    Footer,
  }
}
</script>

<style lang="scss">
  @import "./assets/style/commonstyle.scss";
</style>
