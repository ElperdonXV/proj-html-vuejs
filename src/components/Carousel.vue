<template>
  <div class="carousel m-5">
      <div class="row row-col-3 my-row">
          <div :key="index" v-for="(card, index) in pages[counter].cards" class="col-3 card shadow-lg">
            <img :src="`../assets/${card.img}`" alt="">  
            <h1>{{card.title}}</h1>
            <p>{{card.description}}</p>
          </div>   
      </div>
     <div class="nav m-5">
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
                img: 'logo.png',
                title: 'Consultive Training',
                description: 'With a coach adressing multiple issues that are off balance, affecting your nusiness in various unconsidered ways',
              },
              {
              img: 'en.png',
              title: 'Real Deal Coaching',
              description: 'With a coach adressing multiple issues that are off balance, affecting your nusiness in various unconsidered ways',
              },
              {
              img: 'en.png',
              title: 'Advisor Training Program',
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
  .my-row{
    justify-content: center;
    gap: 20px;
  }
  .nav{
    align-items: center;
    justify-content: center;
    gap: 10px;
    i{
      font-size: 0.5em;
      color: grey;
    }
    .active{
      font-size: 1.5em;
      color: black;
    }
  }
</style>