<template>
  <section class="explore">
      <div class="container">
        <h2 class="mb-4">Let's Dream Big Together</h2>
        <h3>Explore How can I help you</h3>
        <Carousel />
      </div>
  </section>
</template>

<script>
import Carousel from './Carousel.vue';
export default {
    name: 'Explore',
    components: {
        Carousel,
    }
}
</script>

<style lang="scss">
@import "../assets/scss/partials/_variables.scss";
    .explore{
        background-color: $porcelain;
         padding-top: 100px;
        h2,h3{
            text-align: center;
        }
        h2{
            font-weight: 500;
            color: $mountain;
        }
        h3{
            font-size: 2.5em;
            font-weight: 700;
        }
    }
</style>