<template>
  <main>
    <Jumbo />
    <section class="services">
      <div class="container">
        <h2 class="mb-4">Let's Dream Big Togheter</h2>
        <h3>
            We are pioneers of the digital approach, using leading-edge technology to simplify procedures 
            and apply executive coaching in the new age of digitalization.
        </h3>
        <div class="services-list">

        </div>
      </div>
    </section>
  </main>
</template>

<script>
import Jumbo from './Jumbo.vue';
export default {
    name: 'Main',
    components: {
      Jumbo,
    },
    data(){

    },
}
</script>

<style lang="scss">
@import "../assets/scss/partials/_variables.scss";
  .services{
    padding-top: 100px;
    h2,h3{
      text-align: center;
    }
    h2{
      font-weight: 500;
      color: $mountain;
    }
    h3{
      font-weight: 700;
    }
  }
</style>