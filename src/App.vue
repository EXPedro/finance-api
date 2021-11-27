<template>
  <div id="app">
    <!-- Header / -->
    <Container />
  </div>
</template>

<script>
//import Header from './components/header'
import Container from './components/container'

export default {
  name: 'App',
  components: {
    //Header,
    Container,
  }
}
</script>

<style>
  :root{
    --corLetraHeader: #927328;
    --corHeader: #8B92B6;
    --corCard: #e0c583;
    /* --corFundoContainer: #BDC1D7; */
    --corFundoContainer: #FFF5DB; 
    --corBorda: #B8994E;      
    --corSombraBorda: #927328;  
  }
  body{
    margin: 0px;
    padding: 0px;

    overflow-y: auto;
    overflow-x: hidden;
  }
</style>
