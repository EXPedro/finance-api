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
        :abertura= "ativo.abertura" />  
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
          figura: 'itsa4.png',
          nome: 'ITSA4',
          preco: 9.83,
          abertura: 9.89,
        },
        {
          id: 1,
          figura: 'movida.png',
          nome: 'MOVI3',
          preco: 17.17,
          abertura: 17.52,
        },
        {
          id: 2,
          figura: 'egie3.png',
          nome: 'EGIE3',
          preco: 39.00,
          abertura: 38.75,
        },
        {
          id: 3,
          figura: 'taesa.png',
          nome: 'TAEE11',
          preco: 35.94,
          abertura: 35.70,
        },
        {
          id: 4,
          figura: 'magalu.png',
          nome: 'MGLU3',
          preco: 8.06,
          abertura: 8.48,
        },
        {
          id: 5,
          figura: 'irbr3.png',
          nome: 'IRBR3',
          preco: 4.14,
          abertura: 4.07,
        },
        {
          id: 6,
          figura: 'itau.png',
          nome: 'ITUB3',
          preco: 29.78,
          abertura: 20.36,
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

        background-color: var(--corContainer);
        /*background-image: url('../assets/img/moeda.svg'); */

        overflow-y: auto;
    }
	
</style>