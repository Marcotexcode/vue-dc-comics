<template>

  <div id="app">

    <Header/>

    <main>

      <MainTop/>

      <MainBottom/>

    </main>

    <footer>

      <FooterTop/>

      <FooterBottom/>

    </footer>
    
  </div>

</template>

<script>

  import Header from './components/Header.vue'
  import MainTop from './components/MainTop.vue'
  import MainBottom from './components/MainBottom.vue'
  import FooterTop from './components/FooterTop.vue'
  import FooterBottom from './components/FooterBottom.vue'





  export default {

    name: 'App',

    components: {
      
      Header,
      MainTop,
      MainBottom,
      FooterTop,
      FooterBottom

    }

  }

</script>

<style lang="scss">

@import '../src/style/commons.scss';


// #app {
//   font-family: Avenir, Helvetica, Arial, sans-serif;
//   -webkit-font-smoothing: antialiased;
//   -moz-osx-font-smoothing: grayscale;
//   text-align: center;
//   color: #2c3e50;
//   margin-top: 60px;
// }
</style>
