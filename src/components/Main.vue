<template>
  <main>
    <Jumbo />
    <Services />
    <Explore />
    <Cards />
  </main>
</template>

<script>
import Jumbo from './Jumbo.vue';
import Services from './Services.vue';
import Explore from './Explore.vue';
import Cards from './Cards.vue';
export default {
    name: 'Main',
    components: {
      Jumbo,
      Services,
      Explore,
      Cards,
    },
    data(){

    },
}
</script>

<style lang="scss">
</style>