<template>
  <section id="sponsor">

    <div class="container">

      <div class="row box-title-sponsors">
        <h3 class="title-sponsors">Sponsors</h3>
        <p class="description-sponsors">Maecenas faucibus mollis interdum. Nullam id dolor id nibh ultricies vehicula ut id elit.</p>
      </div>

      <div class="row box-image-sponsors">
        <figure v-for="(el, i) in sponsorList" :key="i" class="item-sponsors">
          <img :src="el.img" alt="">
        </figure>
      </div>

    </div>

  </section>
</template>

<script>
export default {
  name: 'MainSponsor',
  data() {
    return {
      sponsorList: [
        {
          img: require('../assets/img/banner-1.jpg')
        },
        {
          img: require('../assets/img/banner-2.jpg')
        },
        {
          img: require('../assets/img/banner-3.jpg')
        },
        {
          img: require('../assets/img/banner-4.jpg')
        },
        {
          img: require('../assets/img/banner-5.jpg')
        },
        {
          img: require('../assets/img/banner-6.jpg')
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">

@import '../assets/scss/common.scss';

section {

  padding: 80px 10px;
  background-color: #f6f6f6;

  .container {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 30px;

    .box-title-sponsors {
      text-align: center;

      .title-sponsors {
        text-transform: uppercase;
        font-size: 27px;
        padding-bottom: 20px;
      }

      .description-sponsors {
        color: $gray;
        max-width: 60%;
        margin: 0 auto;
        padding-bottom: 25px;
      }
    }

    .box-image-sponsors {
      display: flex;
      justify-content: center;
      gap: 20px;

      .item-sponsors {
        width: calc( (100% / 6) - 20px );
      }
      
    }

  }

}

</style>
