<template>
  <div class="card">
    <!-- img :src= "figura" class="imagem" / -->
    <img :src="require(`@/assets/img/${figura}`)"  class="imagem">
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

    border-radius: 100%;
    border-style: solid;
    border-color: var(--corBorda);

    /*box-shadow porperties size x, size y, blur, radius, color*/
    box-shadow: 8px 8px 5px var(--corSombraBorda);
  }

  .card:hover{
    transform: scale(1.05);
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