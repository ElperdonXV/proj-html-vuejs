<template>
  <section class="newsletter">
      <div class="container">
          <div class="row">
              <div class="col d-flex justify-content-center align-items-center">
                  <div class="circle">
                  </div>
              </div>
              <div class="col d-flex flex-column justify-content-center align-items-center mycol">
                <h1 class="mb-4">Subscribe <span>Newsletters</span></h1>
                <p class="mb-4">Enter your email address to register to our nrewsletter subscription delivered on a regular basis!</p>  
                <div class="input-group mb-3">
                    <input type="email" class="form-control my-input" placeholder="Enter your email" aria-label="Enter your email" aria-describedby="button-addon2">
                    <button class="btn my-btn" type="button" id="button-addon2">Subscribe</button>
                </div>
              </div>
              <div class="col d-flex justify-content-center align-items-center relative">
                  <img src="../assets/maxcoach-shape-09.png" alt="">
                  <div class="absolute">
                      <img src="../assets/maxcoach-shape-02.png" alt="">
                  </div>
              </div>
          </div>
      </div>
  </section>
</template>

<script>
export default {
name: 'Newsletter'
}
</script>

<style lang="scss">
@import "../assets/scss/partials/_variables.scss";
    .newsletter{
        padding: 150px 0;
        .circle{
            width: 50px;
            height: 50px;
            border-radius: 50%;
            border: 3px solid $mountain;
            justify-self: flex-end;
        }
        .relative{
            position: relative;
            .absolute{
                position: absolute;
                bottom: 0;
                left: 140px;
            }
        }
        .mycol{
            text-align: center;
            flex-grow: 2;
            h1{
                font-size: 3em;
                font-weight: 800;
                span{
                    color: $mountain;
                    font-weight: 500;
                }
            }
            p{
                font-size: 1.2em;
                line-height: 1.6em;
            }
            .my-input{
                background-color: $mygray;
                border: none;
                padding: 10px;
            }
            .my-input:hover, .my-btn:active, .my-btn:focus{
                box-shadow: none;
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
</style>