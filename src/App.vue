<template>
  <div id="app">
    <Header />
    <Container />
  </div>
</template>

<script>
import Header from './components/header'
import Container from './components/container'

export default {
  name: 'App',
  components: {
    Header,
    Container,
  }
}
</script>

<style>
  :root{
    --corLetraHeader: yellow;
    --corHeader: blue;
    --corCard: white;
    --corFundoContainer: aqua;     
  }
  body{
    margin: 0px;
    padding: 0px;
  }
</style>
