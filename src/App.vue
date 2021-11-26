<template>
  <div id="app">
    <Header />
  </div>
</template>

<script>
import Header from './components/header'

export default {
  name: 'App',
  components: {
    Header,
  }
}
</script>

<style>
  :root{
    --corLetraHeader: yellow;
    --corHeader: blue;
  }
  body{
    margin: 0px;
    padding: 0px;
  }
</style>
