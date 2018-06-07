<template>
  <div id="app">
    <Header title="Gusto !" subtitle="Italiano Ristorante" />
    <HelloWorld msg="Que bella...!"/>
    <Footer/>
  </div>
</template>

<script>
    import HelloWorld from './components/HelloWorld.vue'
    import Header from './components/Header.vue'
    import Footer from './components/Footer.vue'

    export default {
        name: 'app',
        components: {
            Header,
            HelloWorld,
            Footer
        }
    }
</script>

<style>
  #app {
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }

</style>
