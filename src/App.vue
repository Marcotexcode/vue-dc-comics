<template>

  <div id="app">

    <Header/>

    <main>

      <MainTop/>

      <MainBottom/>

    </main>
    
  </div>

</template>

<script>

  import Header from './components/Header.vue'
  import MainTop from './components/MainTop.vue'
  import MainBottom from './components/MainBottom.vue'



  export default {

    name: 'App',

    components: {
      
      Header,
      MainTop,
      MainBottom

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
