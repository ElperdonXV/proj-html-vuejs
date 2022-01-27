<template>
  <div class="carousel m-5">
      <div class="row row-col-3 my-row">
          <div :key="index" v-for="(card,index) in pages[counter].cards" class="card mb-3 shadow col-3">
              <img :src="require(`../assets/${card.src}`)" alt="">
              <div class="card-body">
                <h1 class="m-2">{{card.title}}</h1>
                <p class="m-2">{{card.description}}</p>
               </div>
              <div class="card-footer bg-transparent">
                <a href="#">Discover now &rarr;</a>
              </div>
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
                src: 'home-business-service-slide-01-480x298.jpg',
                title: 'Consultive Training',
                description: 'With a coach adressing multiple issues that are off balance, affecting your nusiness in various unconsidered ways',
              },
              {
                src: 'home-business-service-slide-02-480x298.jpg',
                title: 'Real Deal Coaching',
                description: 'With a coach adressing multiple issues that are off balance, affecting your nusiness in various unconsidered ways',
              },
              {
                src: 'home-business-service-slide-03-480x298.jpg',
                title: 'Advisor Training Program',
                description: 'With a coach adressing multiple issues that are off balance, affecting your nusiness in various unconsidered ways',
              },
            ], 
          },
          {
            cards:[
              {
                src: 'home-business-service-slide-02-480x298.jpg',
                title: 'hei',
                description: 'no',
              }
            ]
          },
          {
            cards: [
              {
                src: 'home-business-service-slide-01-480x298.jpg',
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
@import "../assets/scss/partials/_variables.scss";
  .my-row{
    justify-content: center;
    gap: 20px;
  }
  .card{
    text-align: center;
    padding: 0 !important;
    h1{
      font-size: 1.2em;
      font-weight: 700;
    }
    p{
      color: $boulder;
    }
    .card-footer{
      width: 100%;
      a{
        text-decoration: none;
        font-weight: 700;
        color: $mountain;
      }
      padding: 15px;
    }
    .card-footer:hover{
      background-color: $mountain!important;
      border: none!important;
      cursor: pointer;
      a{
        color: white;
      }
    }
  }
  .nav{
    align-items: center;
    justify-content: center;
    gap: 10px;
    i{
      font-size: 0.5em;
      color: grey;
      cursor: pointer;
    }
    .active{
      font-size: 1.5em;
      color: black;
    }
  }
</style>