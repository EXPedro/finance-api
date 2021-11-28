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
  },
  data() {
    return {
      showEdit: true,
    }
  },
}
</script>

<style>
  :root{
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
