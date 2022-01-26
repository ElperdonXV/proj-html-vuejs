<template>
  <main>
    <Jumbo />
    <Services />
    <Explore />
    <Cards />
    <Business />
  </main>
</template>

<script>
import Jumbo from './Jumbo.vue';
import Services from './Services.vue';
import Explore from './Explore.vue';
import Cards from './Cards.vue';
import Business from './Business.vue';
export default {
    name: 'Main',
    components: {
      Jumbo,
      Services,
      Explore,
      Cards,
      Business,
    },
    data(){

    },
}
</script>

<style lang="scss">
</style>