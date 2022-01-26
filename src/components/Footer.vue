<template>
  <footer>
    <div class="container">
      <div class="row mb-5">
        <div class="col sx">
          <h1 class="mb-3">Address</h1>
          <h2>382 NE 191st ST # 87394 Miami, FL 33179-3899</h2>
          <h2>+1(305)547-9909 (9am - 5pm EST, Monday -Friday</h2>
          <h2>support@maxcoach.com</h2>
          <div class="social d-flex gap-5 mt-5">
            <a href=""><i class="fab fa-facebook-square"></i></a>
            <a href=""><i class="fab fa-twitter"></i></a>
            <a href=""><i class="fab fa-instagram"></i></a>
            <a href=""> <i class="fab fa-linkedin"></i></a>
          </div>
        </div>
        <div class="col">
          <div class="row gap-5">
            <div class="col">
              <h1 class="mb-3">Explore</h1>
              <ul>
                <li><a href="">Start here</a></li>
                <li><a href="">Blog</a></li>
                <li><a href="">About us</a></li>
              </ul>
            </div>
            <div class="col">
              <ul class="without-heading">
                <li><a href="">Success story</a></li>
                <li><a href="">Courses</a></li>
                <li><a href="">Contact us</a></li>
              </ul>
            </div>
            <div class="col">
              <h1 class="mb-3">Information</h1>
              <ul>
                <li><a href="">Membership</a></li>
                <li><a href="">Purchase guide</a></li>
                <li><a href="">Privacy policy</a></li>
                <li><a href="">Terms of service</a></li>
              </ul>
            </div>
          </div>
        </div>
      </div>
      <h4 class="mt-4 copy">&copy; 2020 Maxcoach. All Rights Reserved</h4>
    </div>
  </footer>
</template>

<script>
export default {
    name: 'Footer',
    data(){

    },
}
</script>

<style lang="scss">
@import "../assets/scss/partials/_variables.scss";
  footer{
    padding: 100px 0;
    background-color: black;
    h1{
        color: white;
        font-size: 1.5em;
        font-weight: 700;
      }
    ul{
      list-style: none;
      padding: 0!important;
      li{
        margin-bottom: 1em;
        a{
          color: $boulder;
          text-decoration: none;
        }
      }
      li:hover a {
        color: white;
      }
    }
    .sx{
      h2, i{
        color: $boulder;
      }
      h2{
        font-size: 1em;
        margin-bottom: 1.2em;
        font-weight: 500;
      }
      i{
        font-size: 1.8em;
      }
      i:hover{
        color: white;
        cursor: pointer;
      }

    }
    .copy{
      color: $boulder;
      text-align: center;
      font-size: 1.2em;
    }
    .without-heading{
      margin-top: 2.5em;
    }
  }
</style>