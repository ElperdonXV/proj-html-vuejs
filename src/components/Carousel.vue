<template>
  <div class="carousel">
      <div class="row row-col-3">
          <div :key="index" v-for="(card, index) in pages[counter].cards" class="col-3 card">
            <img :src="`../assets/ + ${card.img}`" alt="">  
            <h1>{{card.title}}</h1>
            <p>{{card.description}}</p>
          </div>   
      </div>
     <div class="nav">
        <i @click="clickCircle(index)" :key="index" v-for="(circle, index) in pages" class="fas fa-circle" :class="(counter == index) ? 'active' : ''"></i>
      </div>
  </div>
</template>

<script>
export default {
    name: 'Carousel',
    data(){
      return{
        counter: 0,
        pages: [
          {
            cards: [
              {
                img: 'en.png',
                title: 'Consultive Training',
                description: 'With a coach adressing multiple issues that are off balance, affecting your nusiness in various unconsidered ways',
              },
              {
              img: 'en.png',
              title: 'Consultive Training',
              description: 'With a coach adressing multiple issues that are off balance, affecting your nusiness in various unconsidered ways',
              },
              {
              img: 'en.png',
              title: 'Consultive Training',
              description: 'With a coach adressing multiple issues that are off balance, affecting your nusiness in various unconsidered ways',
              },
            ], 
          },
          {
            cards:[
              {
                img: '',
                title: 'hei',
                description: 'no',
              }
            ]
          },
          {
            cards: [
              {
                img: '',
                title: 'si',
                description: 'si',
              } 
            ]
          },
        ],
      }
    },
    methods: {
      clickCircle: function (index) {
                this.counter = index;
            },
    }
}
</script>

<style lang="scss">

</style>