<template>
  <section id="presentation">

    <div class="container">

      <div class="row">
        <div>
          <h3>Presentation</h3>
        </div>
        <div>
          <figure class="video-presentation">
            <img src="../assets/img/461365506.webp" alt="">
          </figure>
        </div>
        <div class="vimeo-bar">
          <i class="fa-solid fa-play"></i>
          <div class="bar"></div>
          <i class="fa-solid fa-volume-high"></i>
          <i class="fa-solid fa-gear"></i>
          <p>Vimeo</p>
          <div class="time">1:01:26</div>
        </div>
      </div>

      <div class="row row-twitter">
        <div>
          <h3>Twitter Feed</h3>
        </div>
        <div class="box-twitter">
          <div>
            <i class="fa-brands fa-twitter"></i>
          </div>
          <div>
            <p class="description-twitter">Stand out and be vibrant with some of the best bright and bold templates on <span>@Envato</span> Elements. And add a splash of c... <span>https://t.co/jFsnzEJK7</span></p>
            <p class="time-twitter">3 Days ago</p>
          </div>
        </div>
        <div class="box-twitter">
          <div>
            <i class="fa-brands fa-twitter"></i>
          </div>
          <div>
            <p class="description-twitter">Do you need to delivery the perfect presentation or creative pitch? Sure, your ideas and plan need to be on-point, b <span>https://t.co/nCmvsJVDpW</span></p>
            <p class="time-twitter">9 Days ago</p>
          </div>
        </div>
        <div class="box-twitter">
          <div>
            <i class="fa-brands fa-twitter"></i>
          </div>
          <div>
            <p class="description-twitter">Cut yourself a piece of the BFCM sales pie with a solid marketing plan. Here are 5 ways to optimize your content fo... <span>https://t.co/UZfKHshEOT</span></p>
            <p class="time-twitter">11 Days ago</p>
          </div>
        </div>
      </div>

    </div>

  </section>
</template>

<script>
export default {
  name: 'MainPresentation',
  
}
</script>

<style scoped lang="scss">

@import '../assets/scss/common.scss';

section {

  padding: 80px 10px;

  .container {
    display: flex;
    justify-content: center;
    gap: 40px;
  }

  .row {
    width: 50%;
    position: relative;

    .vimeo-bar {
      background-color: rgba($color: black, $alpha: 0.8);
      color: $white;
      display: flex;
      padding: 10px;
      gap: 15px;
      border-top-left-radius: 8px;
      border-bottom-left-radius: 8px;
      position: relative;
      position: absolute;
      bottom: 20px;
      left: 5%;
      right: -0%;

      .bar {
        flex-grow: 1;
        border: 1px solid white;
      }

      i {
        cursor: pointer;
      }

      .time {
        position: absolute;
        top: -15px;
        left: 7%;
        background-color: $white;
        color: $black;
        padding: 2px;
        font-size: 12px;
      }

      .fa-play {
        padding-left: 10px;
        font-size: 18px;
      }


    }

    .video-presentation {
      width: 80%;
      margin-top: 40px;
      margin-left: 10%;
    }

    h3 {
      text-transform: uppercase;
      font-size: 22px;
    }

  }

  .row-twitter {

    .box-twitter {
      display: flex;
      gap: 20px;
      padding-top: 40px;
    }

    i {
      color: #47bdee;
    }

    .description-twitter {
      color: $gray;
      font-size: 14px;
      padding-bottom: 10px;

      span {
        color: $sienna;
        cursor: pointer;
      }
    }

    .time-twitter {
      color: $gray;
      font-size: 12px;
    }
    
  }

}

@media all and (max-width: 444px) {

  section {

    .container {
      flex-wrap: wrap;

      .vimeo-bar {
        display: none;
      }
    }

  }

}

</style>
