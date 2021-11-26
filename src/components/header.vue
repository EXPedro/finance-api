<template>
  <div class= 'header'>
    <h1>Economia</h1>
  </div>
</template>

<script>
export default {
  name: 'Header',
  components:{
  },
}
</script>

<style>
	.header{
		width: 100vw;
		height: 10vh;
		color: var(--corLetraHeader);
		background-color: var(--corHeader);

    position: fixed;
		
		display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    z-index: 9999;
	}
</style>