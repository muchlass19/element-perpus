<template>
  <div>
    <NavSide></NavSide>
    <Carousel></Carousel>
    <Card></Card>  
  </div>
</template>

<script>
import NavSide from '~/components/content/navside.vue';
import Carousel from '~/components/content/carousel.vue';
import Card from '~/components/content/card.vue';
import Logo from '~/components/Logo.vue';

export default {
  components: {
    Logo,
    NavSide,
    Carousel,
    Card,
  }
}
</script>

<style>
  
</style>