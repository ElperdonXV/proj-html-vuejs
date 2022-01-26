<template>
  <section class="review">
      <div class="container-fluid">
          <h2 class="mb-4">People are praising Maxcoach</h2>
          <h3 class="mb-5">What make they love us?</h3>
          <div class="row gap-4">
              <div :key="index" v-for="(review,index) in reviews" class="col card p-3" :class="(review.active != false) ? '' : 'opacity'">
                  <h4 class="mb-4">{{review.title}}</h4>
                  <p class="mb-4">{{review.text}}</p>
                  <div class="row align-items-center">
                      <div class="col avatar mt-2">
                        <img src="../assets/testimonial-avata-03.jpg" alt="">
                      </div>
                      <div class="col d-flex flex-column">
                          <h5 class="mb-2">{{review.name}}</h5>
                          <h6>{{review.about}}</h6>
                      </div>
                  </div>
              </div>
          </div>
          <div class="nav m-5">
            <i @click="clickCircle(index)" :key="index" v-for="(circle, index) in reviews" class="fas fa-circle" :class="(reviews[index].active != false) ? 'active' : ''"></i>
        </div>
      </div>
  </section>
</template>

<script>
export default {
name: 'Review',
data (){
    return{
        counter: 0,
        reviews: [
            {
                name: 'Mina Hollace',
                about: '/Freelancer',
                title: 'High level of efficiency an scientific',
                text: 'There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words which',
                img: '',
                active: false,
            },
            {
                name: 'Madley Pondor',
                about: '/IT Specialist',
                title: 'Professional team of specialists and passionate',
                text: 'There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words which',
                img: '',
                active: true,
            },
            {
                name: 'Florence Themes',
                about: '/Multimedia Admin',
                title: 'A choice of quality for peaple with special needs',
                text: 'There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words which',
                img: '',
                active: false,
            },
        ]
    }
}
}
</script>

<style lang="scss">
@import "../assets/scss/partials/_variables.scss";
    .review{
        padding: 100px 0;
        background-color: $mygray;
        h2,h3{
            text-align: center;
        }
        h2{
            font-weight: 500;
            color: $mountain;
            font-size: 1.5em;
        }
        h3{
            font-weight: 700;
            font-size: 2.2em;
        }
        .card{
            text-align: left;
            border: none;
            padding: 40px!important;
            h4{
                color: $tuna;
                font-weight: 700;
                font-size: 1.3em;
            }
            p{
                color: black;
            }
            .avatar{
                flex-grow: 0;
                img{
                    border-radius: 50%;
                    width: 80px;
                }   
            }
            h5{
                text-transform: uppercase;
                color: $tuna;
                font-weight: 700;
                font-size: 1em;
            }
            h6{
                font-size: 0.8em;
                color: $boulder;
            }
        }
        .opacity{
            opacity: 50%;
        }
    }
    .container-fluid{
        padding: 0 80px !important;
    }
</style>