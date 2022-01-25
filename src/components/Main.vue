<template>
  <main>
    <Jumbo />
    <Services />
    <Explore />
  </main>
</template>

<script>
import Jumbo from './Jumbo.vue';
import Services from './Services.vue';
import Explore from './Explore.vue';
export default {
    name: 'Main',
    components: {
      Jumbo,
      Services,
      Explore,
    },
    data(){

    },
}
</script>

<style lang="scss">
</style>