<template>
  <div class="card">
    <img src= "../assets/money-increase.png" alt="figura" class="imagem"/>
    <div>{{ nome }}</div>
    <div>Preço: {{ preco }}</div>
    <div>Abertura: {{ abertura }}</div>
    <div class= "canto">{{ variacao }} %</div>
  </div>
</template>

<script>
export default {
  name: 'Card',
  props:{
    figura: String,
    nome: String,
    preco: Number,
    abertura: Number,
    variacao: Number,
  },
  components:{

  },
}
</script>

<style>
  .card{
    width: 13.5vw;
    height: 33vh;
    background-color:var(--corCard);

    display: flex;
    flex-direction: column;
    align-items: center;
    /*justify-content: end;  /*sera q figura fica no meio?*/
    justify-content: center;
        
    margin-top: 8px;
    padding-top: 8px;
  }

  .canto{
    position: relative;
    left: 45px; 
  }	

  .imagem{
    position: relative;
    bottom: 5px;
    width: 5vw;
    height: auto;
  }
</style>