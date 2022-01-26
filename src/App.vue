<template>
  <div class="relative" id="app">
    <Header />
    <Main />
    <Footer />
    <a href="#" class="nav-circle">
      <i class="fas fa-arrow-up"></i>
    </a>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap";
@import "./assets/scss/partials/_variables.scss";
@import url('https://fonts.googleapis.com/css2?family=Catamaran:wght@300;400;500;600;700&family=PT+Sans+Narrow:wght@400;700&display=swap');
.relative{
  position: relative;
}
#app{
  max-width: 100%;
  overflow: hidden;
  .nav-circle{
    position: fixed;
    bottom: 20px;
    right: 30px;
    width: 60px;
    height: 60px;
    display: flex;
    align-items: center;
    justify-content: center;
    text-decoration: none;
    border-radius: 50%;
    background-color: $mountain;
    padding: 10px;
    i{
      color: white;
      font-size: 2em;
    }
  }
}
</style>
