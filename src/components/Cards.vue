<template>
  <section class="cards">
      <div class="container">
        <h2 class="mb-4">Let's Dream Big Togheter</h2>
        <h3>Explore How can I help you</h3>
        <div class="row justify-content-center gap-4 mt-5">
          <div class="card col relative">
            <img src="../assets/course-02-443x600.jpg" alt="">
            <div class="text">
              <h4>$40.00</h4>
              <h5>Learning to write as a Professional Author</h5>
              <div class="bottom m-1">
                <span><i class="far fa-file-alt"></i> 20 Lesson</span>
                <span><i class="far fa-user"></i> 50 Users</span>
                <p class="mt-2">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nemo.</p>
              </div>
            </div>
          </div>
          <div class="card col relative">
            <img src="../assets/stock-full-hd-03-443x600.jpg" alt="">
            <div class="text">
              <h4>Free</h4>
              <h5>Customer-centric-info-tech Strategies</h5>
              <div class="bottom m-1">
                <span><i class="far fa-file-alt"></i> 20 Lesson</span>
                <span><i class="far fa-user"></i> 50 Users</span>
                <p class="mt-2">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nemo.</p>
              </div>
            </div>
          </div>
          <div class="card col relative">
            <img src="../assets/stock-full-hd-04-443x600.jpg" alt="">
            <div class="text">
              <h4>$19.00</h4>
              <h5>Open Programming Courses for Everyone: Python</h5>
              <div class="bottom m-1">
                <span><i class="far fa-file-alt"></i> 20 Lesson</span>
                <span><i class="far fa-user"></i> 50 Users</span>
                <p class="mt-2">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nemo.</p>
              </div>
            </div>
          </div>
          <div class="card col relative">
            <img src="../assets/stock-full-hd-06-443x600.jpg" alt="">
            <div class="text">
              <h4>$26.00</h4>
              <h5>Academic Listening and Note-taking</h5>
              <div class="bottom m-1">
                <span><i class="far fa-file-alt"></i> 20 Lesson</span>
                <span><i class="far fa-user"></i> 50 Users</span>
                <p class="mt-2">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nemo.</p>
              </div>
            </div>
          </div>
        </div>
      </div>
  </section>
</template>

<script>
export default {
    name: 'Cards',
}
</script>

<style lang="scss">
@import "../assets/scss/partials/_variables.scss";
  .cards{
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
      font-size: 2.2em;
    }
    .card{
      .relative{
        position: relative;
      }
      .text{
        position: absolute;
        bottom: 0;
        left: 0;
        padding: 20px;
        text-align: left;
        background: rgb(0,0,0);
        background: linear-gradient(0deg, rgba(0,0,0,0.8) 50%, rgba(0,0,0,0) 100%);
        h4{
          font-size: 1.4em;
          color: $mountain;
          font-weight: 700;
        }
        h5{
          color: white;
          font-size: 1.3em;
          font-weight: 700;
        }
        .bottom{
          display: none;
          span{
            color: white;
            margin-right: 1em;
          }
          p{
            color: white;
          }
        }
      }
    }
    .card:hover .bottom{
      display: block;
    }
  }
</style>