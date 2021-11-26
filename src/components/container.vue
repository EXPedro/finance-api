<template>
  <div class='container'>
    <Card />
    <Card />
    <Card />
    <Card />
    <Card />
    <Card />
    <Card />
  </div>
</template>

<script>
import Card from './card'

export default {
  name: 'Container',
  components:{
    Card,
  },
}
</script>

<style>
    .container{
        width: 100vw;
        height: 90vh;

        position: relative;

        top: 10vh;

        display: grid;
        grid-template-columns: auto auto auto auto auto auto auto;
        justify-content: space-evenly;

        background-color: var(--corFundoContainer);  
    }
	
</style>