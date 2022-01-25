<template>
  <div class="jumbotron d-flex">
      <div class="text">
        <h2 class="mb-4">New Challenges, New Skills</h2>
        <h1 class="mb-4">Build your own life coaching business</h1>
        <p class="mb-2">Whole-Life Business Coaching for commited entrepreneurs</p>
        <button type="button" class="btn my-btn mt-3">Get started today</button>
      </div>
      <div class="bg">
          <img class="avatar" src="../assets/home-business-hero-avatar.png" alt="">
          <img class="world" src="../assets/home-business-hero-global-image.png" alt="">
      </div>
      <div class="right-bar shadow-lg">
          <i class="fas fa-ruler-combined mb-3"></i>
          <i class="far fa-life-ring mb-3"></i>
          <i class="fas fa-book mb-3"></i>
          <i class="fas fa-shopping-cart mb-3"></i>
      </div>
  </div>
</template>

<script>

export default {
name: 'Jumbo',
}
</script>

<style lang="scss">
@import "../assets/scss/partials/_variables.scss";
    .jumbotron{
        height: 700px;
        background-color: $water;
        position: relative;
        padding-left: 400px;
        .text{
            display: inline-block;
            width: 450px;
            align-self: center;
            h2{
                color: $mountain;
                font-weight: 500;
                font-size: 1.7em;
            }
            h1{
                text-transform: uppercase;
                font-weight: 700;
                font-size: 3em;
            }
            .my-btn{
            background-color: $mountain;
            color: white;
            font-weight: 700;
            font-size: 1em;
            padding: 10px;
            }
            .my-btn:hover, .my-btn:active, .my-btn:focus{
                background-color: $tuna;
                box-shadow: none;
            }
        }
        .bg{
            height: 100%;
            .world{
                position: absolute;
                top: 0;
                right: 150px;
                height: 100%;
            }
            .avatar{
                position: absolute;
                bottom: 0;
                right: 400px;
                height: 90%;
                z-index: 3;
            }
        }
        .right-bar{
            padding: 15px 15px 15px 10px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            position: absolute;
            top: 100px;
            right: -10px;
            background-color: white;
            border-radius: 10px;
            i{
                font-size: 1.1em;
            }
        }
    }
</style>