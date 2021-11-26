<template>
  <div class='card'>
    <div>figura</div>
    <div>nome</div>
    <div>preço</div>
    <div class= 'canto'>abertura</div>
    <div class= 'canto'>fechamento</div>
  </div>
</template>

<script>
export default {
  name: 'Card',
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
        justify-content: end;  /*sera q figura fica no meio?*/

        margin-top: 8px;
        padding-top: 8px;
    }

    .canto{
       position: relative;
       left: 42px; 
    }
	
</style>