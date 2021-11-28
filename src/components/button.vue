<template>
  <button class="botao" > </button>
</template>

<script>
export default {
  name: 'Botao',
  
}
</script>

<style>
  .botao{
    width: 50px;
    height: 50px;

    background-image: url("../assets/img/plus-circle.svg");
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    background-color: var(--corContainer);

    position: fixed;
    top: 80vh;
    right: 10%;
    z-index: 99999;

    border-radius: 100%;
    border-color: var(--corBorda);

    transform: scale(2);

    box-shadow: 8px 8px 15px var(--corBorda);
  }
</style>