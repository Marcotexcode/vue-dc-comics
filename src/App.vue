<template>

  <div id="app">

    <Header/>

    <Jumbotron/>

    <main>

      <Sezione1/>

      <Sezione2/>

    </main>

    <footer>

      <FooterTop/>

      <FooterBottom/>

    </footer>
    
  </div>

</template>

<script>

  import Header from './components/Header.vue'
  import Sezione1 from './components/Sezione1.vue'
  import Sezione2 from './components/Sezione2.vue'
  import FooterTop from './components/FooterTop.vue'
  import FooterBottom from './components/FooterBottom.vue'
  import Jumbotron from './components/Jumbotron.vue'






  export default {

    name: 'App',

    components: {
      
      Header,
      Sezione1,
      Sezione2,
      FooterTop,
      FooterBottom,
      Jumbotron

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
