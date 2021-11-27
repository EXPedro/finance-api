<template>
  <div>
    <div class='container' >
      <Card v-for= "ativo in ativos" :key= "ativo.id"
        :figura= 'ativo.figura'
        :nome= 'ativo.nome'
        :preco= 'ativo.preco' 
        :abertura= "ativo.abertura" 
        :variacao= "ativo.variacao" />
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
          figura: 'money-increase.png',
          nome: 'ITSA4',
          preco: 10.22,
          abertura: 10.22,
          variacao: 0.00
        },
        {
          id: 1,
          figura: 'money-increase.png',
          nome: 'MOVI3',
          preco: 31.15,
          abertura: 10.22,
          variacao: 0.00
        },
        {
          id: 2,
          figura: 'money-increase.png',
          nome: 'EGIE3',
          preco: 85.62,
          abertura: 10.22,
          variacao: 0.00
        },
        {
          id: 3,
          figura: 'money-increase.png',
          nome: 'TAEE11',
          preco: 67.79,
          abertura: 10.22,
          variacao: 0.00
        },
        {
          id: 4,
          figura: 'money-increase.png',
          nome: 'MGLU3',
          preco: 56.23,
          abertura: 10.22,
          variacao: 0.00
        },
        {
          id: 5,
          figura: 'money-increase.png',
          nome: 'IRBR3',
          preco: 9.63,
          abertura: 10.22,
          variacao: 0.00
        },
        {
          id: 6,
          figura: 'money-increase.png',
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
        height: auto;

        position: relative;

        /*top: 10vh;  --saiu com remoção header */

        display: grid;
        grid-template-columns: auto auto auto auto auto;
        justify-content: space-evenly;
        /*column-gap: 0vw;*/

        background-color: var(--corFundoContainer);
        /*background-image: url('../assets/img/moeda.svg'); */

        overflow-y: auto;
    }
	
</style>