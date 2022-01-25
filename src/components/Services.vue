<template>
  <section class="services">
      <div class="container p-5">
        <h2 class="mb-4">Let's Dream Big Togheter</h2>
        <h3>
            We are pioneers of the digital approach, using leading-edge technology to simplify procedures 
            and apply executive coaching in the new age of digitalization.
        </h3>
        <div class="services-list p-5">
          <div class="row row-col-3 row-gap">
            <div class="col-4 d-flex">
              <div class="icon">
                <i class="far fa-comment"></i>
              </div>
              <div class="text">
                <h4 class="mb-2">One to One</h4>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Vero quaerat provident optio iure totam aperiam dolor in facilis quos ad, nihil aspernatur, doloremque est reiciendis illum enim eum non nostrum.</p>
              </div>
            </div>
            <div class="col-4 d-flex">
              <div class="icon">
                <i class="fas fa-globe-europe"></i>
              </div>
              <div class="text">
                <h4 class="mb-2">Anywhere</h4>
                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Officiis iusto dicta provident ab molestias, amet id eos vero, modi facere distinctio voluptatibus doloremque incidunt, explicabo maxime laborum esse quibusdam officia.</p>
              </div>
            </div>
            <div class="col-4 d-flex">
              <div class="icon">
                <i class="far fa-clock"></i>
              </div>
              <div class="text">
                <h4 class="mb-2">On Time</h4>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus eius laudantium suscipit. Maxime atque quia illo ratione mollitia. Dignissimos, quod! Dignissimos nostrum hic tempora dolorem, ratione modi molestiae soluta corporis?</p>
              </div>
            </div>
            <div class="col-4 d-flex">
              <div class="icon">
                <i class="fas fa-desktop"></i>
              </div>
              <div class="text">
                <h4 class="mb-2">Online Courses</h4>
              <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Maxime, aliquid qui voluptatem nobis dignissimos odio fugiat, deserunt rerum ducimus, nihil alias. Recusandae rerum sit, officiis asperiores maiores illo neque eos.</p>
              </div>
            </div>
            <div class="col-4 d-flex">
              <div class="icon">
                <i class="fas fa-assistive-listening-systems"></i>
              </div>
              <div class="text">
                <h4 class="mb-2">Consulting</h4>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Repudiandae ea nihil magnam, dolores voluptates eos quod iusto consequatur porro quidem odio eaque fugiat molestias error non odit quia facilis corporis?</p>
              </div>
            </div>
            <div class="col-4 d-flex">
              <div class="icon">
                <i class="fas fa-cog"></i>
              </div>
              <div class="text">
                <h4 class="mb-2">Self Development</h4>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Inventore rem odio optio quam atque fugit, vero nemo perferendis voluptatum reprehenderit nesciunt libero ab error, necessitatibus nam eos ipsum tenetur adipisci!</p>
              </div>
            </div>
          </div>
        </div>
        <div class="call-to-action">
          <button type="button" class="btn my-btn-outline m-2">Learn more</button>
          <button type="button" class="btn my-btn m-2">Get started today</button>
        </div>
      </div>
    </section>
</template>

<script>
export default {
    name: 'Services',

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
    .call-to-action{
      text-align: center;
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
      .my-btn-outline{
            border: 2px solid $silver;
            color: $mountain;
            font-weight: 700;
            font-size: 1em;
            padding: 10px 50px;
          }
      .my-btn-outline:hover, .my-btn-outline:active, .my-btn-outline:focus{
                border: 2px solid $tuna;
                color: white;
                background-color: $tuna;
                box-shadow: none;
            }           
    }
  }
  .row-gap{
    row-gap: 40px;
  }
  .col-4{
    h4{
      font-weight: 700;
    }
    .icon{
      padding: 0 10px;
      i{
        font-size: 4em;
      }
    }
  }
</style>