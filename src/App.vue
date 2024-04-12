<template>
  <HeaderComponent />
  <HeroComponent />
  <CardList />
  <FooterComponent />
</template>

<script>
  import HeaderComponent from './components/HeaderComponent.vue';
  import HeroComponent from './components/HeroComponent.vue';
  import CardList from './components/CardList.vue';
  import FooterComponent from './components/FooterComponent.vue';
  export default {
    name: 'App',
    components:{
      HeaderComponent,
      HeroComponent,
      CardList,
      FooterComponent
    }
  }
</script>

<style lang="scss" scoped>

</style>