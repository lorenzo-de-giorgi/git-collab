<template>
    <div class="card" >
        <img :src="coktail.strDrinkThumb" class="card-img-top" :alt="coktail.strDrink">
        <div class="card-body">
        <h5 class="card-title">{{ coktail.strDrink }}</h5>
  </div>
</div>
</template>

<script>
    export default {
        name: 'CardComponent',
        props: ['coktail'], 
    }
</script>

<style lang="scss" scoped>

</style>