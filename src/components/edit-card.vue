<template>
  <div class="edit-card">
    <img :src="require(`@/assets/img/${figura}`)"  class="imagem" >
    <div>Ticker: {{ nome }}</div>
    <div>Preço Médio: </div>
    <div>Quantidade: </div>
    <div>Total: </div>
  </div>  
</template>

<script>
export default {
  name: 'EditCard',
  props: {
    figura: String,
    nome: String,
  },
}
</script>

<style>
  .edit-card{
    width: 33vh;
    height: 33vh;
    background-color:var(--corCard);

    /*display: flex;
    flex-direction: column;
    align-items: center;*/

    position: fixed;
    top: 10px;
    left: 40px;
    z-index: 9999;
  }
</style>