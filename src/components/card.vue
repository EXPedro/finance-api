<template>
  <div class="card">
    <img :src="require(`@/assets/img/${figura}`)"  class="imagem">
    <div>{{ nome }}</div>
    <div>Preço: {{ valorPreco() }}</div>
    <div>Abertura: {{ formatData(abertura) }}</div>
    <div class= "canto verde" v-if="variationF() >= 0" >{{ formatData(variationF()) }} %</div>
    <div class= "canto vermelho" v-else >{{ formatData(variationF()) }} %</div>
    <!-- EditCard :preco = "preco" works! / -->
  </div>
</template>

<script>
//import EditCard from './edit-card'

export default {
  name: 'Card',
  props:{
    figura: String,
    nome: String,
    preco: Number,
    abertura: Number,
  },
  components:{
    //EditCard,
  },
  data(){
    return{
      variation: 0,
      cardPreco:0,
    }
  },
  methods:{
    variationF: function() { 
      return this.variation = ((this.preco * 100) / this.abertura) - 100
    },
    formatData: function(aFormatar) {
      return (Math.round(aFormatar * 100) / 100).toFixed(2)
    },
    valorPreco: function(){
      this.cardPreco = this.formatData(this.preco)
      return this.cardPreco
    }
  },
}
</script>

<style>
  .card{
    width: 33vh;
    height: 33vh;
    background-color:var(--corCard);

    display: flex;
    flex-direction: column;
    align-items: center;
    /*justify-content: end;  /*sera q figura fica no meio?*/
    justify-content: center;
        
    margin-top: 8px;
    padding-top: 8px;

    border-radius: 5%;
    /*border-style: solid;*/
    border-color: var(--corBorda);

    font-family: 'Encode Sans', sans-serif;
    font-weight: 900;
    color: var(--corBorda);

    /*box-shadow porperties size x, size y, blur, radius, color*/
    box-shadow: 8px 8px 15px var(--corBorda);
  }

  .card:hover{
    transform: scale(1.05);
  }

  .card:active{
    position: absolute;
    transform: scale(1.5);
    margin-top: 160px;
    left: 40%;
    z-index: 9999;
  }

  .canto{    
    align-self: flex-end;
    position: relative;
    right: 10px;
    margin-top: 18px;
  }	

  .imagem{
    position: relative;
    bottom: 5px;
    width: 67.13px;
    height: auto;
  }

  .verde{
    color: green;
  }

  .vermelho{
    color: red;
  }
</style>