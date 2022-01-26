<template>
  <main>
    <Jumbo />
    <Services />
    <Explore />
    <Cards />
    <Business />
    <Events />
  </main>
</template>

<script>
import Jumbo from './Jumbo.vue';
import Services from './Services.vue';
import Explore from './Explore.vue';
import Cards from './Cards.vue';
import Business from './Business.vue';
import Events from './Events.vue';
export default {
    name: 'Main',
    components: {
      Jumbo,
      Services,
      Explore,
      Cards,
      Business,
      Events,
    },
    data(){

    },
}
</script>

<style lang="scss">
</style>