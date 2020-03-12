<template>
  <div>
  <NavSide />
  <Carousel />
  <ListKat /><br/>
  <Card />      
  </div>
</template>

<script>
import NavSide from '~/components/content/navside.vue';
import Carousel from '~/components/content/carousel.vue';
import Card from '~/components/content/card.vue';
import ListKat from '~/components/content/list-kat.vue'

export default {
  components: {
    NavSide,
    Carousel,
    Card,
    ListKat,
  }
}
</script>

<style>
  
</style>