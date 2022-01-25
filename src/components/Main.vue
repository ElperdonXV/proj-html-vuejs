<template>
  <main>
    <Jumbo />
    <Services />
  </main>
</template>

<script>
import Jumbo from './Jumbo.vue';
import Services from './Services.vue';
export default {
    name: 'Main',
    components: {
      Jumbo,
      Services,
    },
    data(){

    },
}
</script>

<style lang="scss">
</style>