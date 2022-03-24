<template>
  <section id="speakers">

    <div class="container">

      <div class="row title-row">

        <div class="title">
          <h4>Speakers</h4>
        </div>

        <div class="icon-wrapper">
          <i class="fa-solid fa-angle-left"></i>
          <i class="fa-solid fa-angle-right"></i>
        </div>

      </div>

      <div class="row speakers-row">

        <div v-for="(el, i) in speakersList" :key="i" class="speakers-box">
          <div class="box-image">
            <figure>
              <img :src="el.img" alt="">
            </figure>
            <div class="box-icon">
              <i class="fa-brands fa-twitter"></i>
              <i class="fa-brands fa-facebook-f"></i>
              <i class="fa-brands fa-linkedin-in"></i>
            </div>
          </div>
          <div>
            <p class="speaker">{{ el.speaker }}</p>
            <p class="job">{{ el.job }}</p>
          </div>
        </div>

      </div>

    </div>

  </section>
</template>

<script>
export default {
  name: 'MainSpeakers',
  data() {
    return {
      speakersList: [
        {
          img: require('../assets/img/speaker-6.jpg'),
          speaker: 'Patrick Spencer',
          job: 'S&P Analyzer'
        },
        {
          img: require('../assets/img/speaker-5.jpg'),
          speaker: 'Janet Jones',
          job: "Newyork Post's GM"
        },
        {
          img: require('../assets/img/speaker-4.jpg'),
          speaker: 'Michael Dover',
          job: "Starbuck's CEO"
        },
        {
          img: require('../assets/img/speaker-3.jpg'),
          speaker: 'Angelina Holy',
          job: "Maxii's Manager"
        }
      ]
    }
  }
  
}
</script>

<style scoped lang="scss">

@import '../assets/scss/common.scss';

section {

  padding: 60px 10px;
  background-color: #f6f6f6;

  .speakers-row {
    display: flex;
    justify-content: center;
    gap: 30px;

    .speakers-box {
      width: calc( 100% / 4);
      text-align: center;

      .speaker {
        text-transform: uppercase;
        font-weight: 600;
        padding-bottom: 15px;
      }

      .job {
        font-style: italic;
        color: $gray;
      }

      .box-image {
        padding-bottom: 15px;
        position: relative;
      }

    }

  }

  .title-row {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-bottom: 40px;

    .title {
      text-transform: uppercase;
      font-size: 28px;
    }

    .icon-wrapper i {
      padding: 8px 12px;
      border-radius: 4px;
      background-color: $red;
      color: $white;
      margin: 0 5px;
      cursor: pointer;
    }
    
  }

  .box-image:hover figure::after {
    content: '';
    display: block;
    position: absolute;
    top: 0;
    left: 0;
    bottom: 18px;
    right: 0;
    background-color: rgba($color: red, $alpha: 0.5);
  }

  .box-image:hover .box-icon {
    visibility: visible;
  }

  .box-icon {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    color: $white;
    visibility: hidden;

    i {
      padding: 0 10px;
      font-size: 19px;
      cursor: pointer;
    }

  }

}

</style>
