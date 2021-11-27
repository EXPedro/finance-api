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
    /*--corLetraHeader: #927328;
    --corHeader: #8B92B6;
    --corFundoContainer: #BDC1D7; */ 
    --corCard: #E0C583;
    --corContainer: #FFF5DB; 
    --corPenultimoTom: #B8994E;      
    --corBorda: #927328;  
  }
  body{
    margin: 0px;
    padding: 0px;

    overflow-y: auto;
    overflow-x: hidden;
  }
</style>
