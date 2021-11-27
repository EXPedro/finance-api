<template>
  <div>
    <div class='container' >
      <Card v-for= "ativo in ativos" :key= "ativo.id"
        :figura= 'ativo.figura'
        :nome= 'ativo.nome'
        :preco= 'ativo.preco' 
        :abertura= "ativo.abertura" 
        :variacao= "ativo.variacao" />
    </div>
  </div>
</template>

<script>
import Card from './card'

export default {
  name: 'Container',
  components:{
    Card,
  },
  data() {
    return {
      ativos: [
        {
          id: 0,
          nome: 'ITSA4',
          preco: 10.22,
          abertura: 10.22,
          variacao: 0.00
        },
        {
          id: 1,
          nome: 'MOVI3',
          preco: 31.15,
          abertura: 10.22,
          variacao: 0.00
        },
        {
          id: 2,
          nome: 'EGIE3',
          preco: 85.62,
          abertura: 10.22,
          variacao: 0.00
        },
        {
          id: 3,
          nome: 'TAEE11',
          preco: 67.79,
          abertura: 10.22,
          variacao: 0.00
        },
        {
          id: 4,
          nome: 'MGLU3',
          preco: 56.23,
          abertura: 10.22,
          variacao: 0.00
        },
        {
          id: 5,
          nome: 'IRBR3',
          preco: 9.63,
          abertura: 10.22,
          variacao: 0.00
        },
        {
          id: 6,
          nome: 'ITUB3',
          preco: 29.78,
          abertura: 10.22,
          variacao: 0.00
        },
      ]}
  }
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