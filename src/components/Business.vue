<template>
  <section class="business relative">
      <div class="bg relative">
          <div class="decoration">
            <img src="../assets/maxcoach-shape-07.png" alt="" >
        </div>
         <div class="world">
            <img src="../assets/background-map-dots-top-right-transparent.png" alt="">
        </div>
         <div class="container">
          <div class="row align-items-center justify-contents-between gap-5">
              <div class="col flex-grow-0">
                  <div class="youtube relative">
                      <img src="../assets/home-business-video-poster-670x450.jpg" alt="" class="rounded-3">
                      <div class="play">
                          <img src="../assets/icon-youtube-play.png" alt="">
                      </div>
                  </div>
              </div>
              <div class="col-4 z-in">
                  <h2 class="mb-5">To thrive in Business Today, You'll Need a Good Plan</h2>
                  <div :key="index" v-for="(ask,index) in asks" class="dropdown d-flex gap-2">
                      <i @click="click(index)" :class="(ask.active !== true) ? 'far fa-arrow-alt-circle-down' : 'far fa-arrow-alt-circle-up' + ' ' + 'green'"></i>
                      <div class="text">
                          <h3 :class="(ask.active !== true) ? '' : 'green'">{{ask.title}}</h3>
                          <p :class="(ask.active !== true) ? 'none' : 'show'">{{ask.paragraph}}</p>
                      </div>
                  </div>
              </div>
          </div>
      </div>
      </div>
  </section>
</template>

<script>
export default {
    name: 'Business',
    data(){
        return{
            asks: [
                {
                    title: 'How can we help?',
                    paragraph: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Similique doloribus nostrum, ullam illo aperiam ex omnisab quae id consequatur atque animi repudiandae quis, obcaecati maiores autem pariatur illum alias?',
                    active: true,
                },
                {
                    title: 'Why would I need a business COACH?',
                    paragraph: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Similique doloribus nostrum, ullam illo aperiam ex omnisab quae id consequatur atque animi repudiandae quis, obcaecati maiores autem pariatur illum alias?',
                    active: false,
                },
                {
                    title: 'What is one-on-one coaching?',
                    paragraph: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Similique doloribus nostrum, ullam illo aperiam ex omnisab quae id consequatur atque animi repudiandae quis, obcaecati maiores autem pariatur illum alias?',
                    active: false,
                },
            ]
        }
    },
    methods: {
        click(index){
            if (this.asks[index].active != true){
                this.asks[index].active = true;
            }
            else{
                this.asks[index].active = false;
            }
        }
    }
}
</script>

<style lang="scss">
@import "../assets/scss/partials/_variables.scss";
    .relative{
            position: relative;
        }
    .business{
        background-color: $charade;
        .container{
            padding: 150px 0;
        }
        .play{
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
        }
        .world{
            position: absolute;
            top: 0px;
            right: 0px;
            z-index: 0;
        }
        .decoration{
            position: absolute;
            bottom: 70px;
            left: 170px;
            z-index: 0;
        }
        .z-in{
            z-index: 4;
            h2,h3,p,i {
                color: white;
            }
            h2{
                font-size: 2.5em;
                font-weight: 700;
            }
            i{
                font-size: 1.5em;
                padding-top: 5px;
                cursor: pointer;
            }
            .dropdown{
                padding: 15px;
                border-bottom: 1px solid rgba($color: #ebebeb, $alpha: 0.3);
            }
            .none{
                display: none;
            }
            .show{
                display: block;
            }
            .green{
                color: $mountain;
            }
        }
    }    
</style>