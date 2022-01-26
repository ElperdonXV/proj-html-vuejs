<template>
  <section class="events">
      <div class="container">
          <h2 class="mb-4">Wanna transform your life?</h2>
          <h3 class="mb-5">Upcoming Events</h3>
          <div class="row justify-content-center gap-4">
              <div :key="index" v-for="(event,index) in events" class="col-5 d-flex event justify-content-between rounded-3">
                  <div class="sx">
                      <i class="fas fa-map-marker-alt me-2"></i>
                      <span>{{event.location}}</span>
                      <h4 class="mt-2">{{event.description}}</h4>
                  </div>
                  <div class="dx d-flex flex-column align-items-center">
                      <h3>{{event.day}}</h3>
                      <h4>{{event.month}}</h4>
                      <button type="button" class="btn my-btn mt-3">Get ticket</button>
                  </div>
              </div>
          </div>
          <p class="mt-5">Excited about our event? <a href="">View all events &rarr;</a></p>
      </div>
  </section>
</template>

<script>
export default {
    name: 'Events',
    data(){
        return{
            events: [
                {
                    location: 'Texas, US',
                    description: 'Storytelling Workshop',
                    day: '22',
                    month: 'NOV',
                },
                {
                    location: 'New York, US',
                    description: 'Painting Art Contest 2020',
                    day: '10',
                    month: 'OCT',
                },
                {
                    location: 'Hamburg, Germany',
                    description: 'International Art Fair 2020',
                    day: '23',
                    month: 'NOV',
                },
                {
                    location: 'Illinois, US',
                    description: 'Street Performance: Call for Artist',
                    day: '15',
                    month: 'DEC',
                },
                {
                    location: 'Illinois, US',
                    description: 'Consumer Food Safety Education Conference',
                    day: '22',
                    month: 'JUL',
                },
                {
                    location: 'Dubai',
                    description: 'How meditation improve your mental healt?',
                    day: '12',
                    month: 'AUG',
                }
            ]
        }
    }
}
</script>

<style lang="scss">
@import "../assets/scss/partials/_variables.scss";
.events{
    padding: 150px 0;
    h2,h3,p{
      text-align: center;
    }
    h2{
      font-weight: 500;
      color: $mountain;
    }
    h3{
      font-weight: 700;
      font-size: 2.2em;
    }
    .event{
        padding: 25px;
        background-color: $mygray;
        .sx{
            max-width: 200px;
            i,span{
                color: $boulder;
            }
            span{
                font-size: 1em;
                font-weight: 600;
            }
            h4{
                font-size: 1.5em;
                font-weight: 700;
            }
            
        }
        .dx{
            h3{
                color: $mountain;
                font-size: 3.5em;
                font-weight: 500;
            }
            h4{
                font-size: 1.2em;
                font-weight: 700;
            }
            .my-btn{
            background-color: $mountain;
            color: white;
            font-weight: 700;
            font-size: 1em;
            padding: 10px 50px;
            }
            .my-btn:hover, .my-btn:active, .my-btn:focus{
                background-color: $tuna;
                box-shadow: none;
            }
        }
    }
    p{
        font-size: 1.1em;
        font-weight: 600;
        a{
            color: $mountain;
            font-weight: 800;
        }
    }
}
</style>