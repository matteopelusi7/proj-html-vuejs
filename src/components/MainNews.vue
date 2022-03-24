<template>
  <section id="news">

    <div class="container">

      <div class="row title-row">

        <div class="title-box">
          <h4 class="title">Recent news</h4>
        </div>

        <div class="more-info">
          <p>Read All News</p>
        </div>

      </div>

      <div class="row row-news">

        <div v-for="(el, i) in newsList" :key="i" class="box-news">
          <figure class="img">
            <img :src="el.img" alt="">
            <div class="stick-news">
              <i class="fa-solid fa-volume-high"></i>
              <p>Sticky Post</p>
            </div>
          </figure>
          <div>
            <p class="data-post">{{ el.post }}</p>
            <h4 class="title-news">{{ el.title }}</h4>
            <p class="description-news">{{ el.description }}</p>
            <p class="more-info">{{ el.more }}</p>
          </div>
        </div>

      </div>

    </div>

  </section>
</template>

<script>
export default {
  name: 'MainNews',
  data() {
    return {
      newsList: [
        {
          img: require('../assets/img/photodune-7770665-two-white-coffee-mug-with-diy-decoration-o (2).jpg'),
          post: '03 Dec 2013 / 0 comments',
          title: 'Sedial eiusmod tempor',
          description: 'Lorem ipsum dolor sit amet, consectetur elit, sed eiusmod tempor incidunt ut labore et dolore magna aliqua idque Caesaris facere voluntate liceret: sese habere...',
          more: 'Read More'
        },
        {
          img: require('../assets/img/photodune-8797753-multiethnic-people-with-startup-business-t (2).jpg'),
          post: '03 Dec 2013 / 2 comments',
          title: 'Donec luctus imperdiet',
          description: 'Lorem ipsum dolor sit amet, consectetur elit, sed eiusmod tempor incidunt ut labore et dolore magna aliqua idque Caesaris facere voluntate liceret: sese habere...',
          more: 'Read More'
        },
        {
          img: require('../assets/img/photodune-8522811-speaker-at-business-conference-and-present (2).jpg'),
          post: '03 Dec 2013 / 2 comments',
          title: 'Magna pars studiorum',
          description: 'Lorem ipsum dolor sit amet, consectetur elit, sed eiusmod tempor incidunt ut labore et dolore magna aliqua idque Caesaris facere voluntate liceret: sese habere...',
          more: 'Read More'
        },
      ]
    }
  }
}
</script>

<style scoped lang="scss">

@import '../assets/scss/common.scss';

section {

  padding: 60px 10px;

  .description {
    color: $gray;
    max-width: 55%;
    padding-left: 60px;
  }

  .more-info {
    color: $sienna;
    font-style: italic;
    cursor: pointer;
  }

  .title-box {
    display: flex;
    align-items: center;
  }

  .title-row {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding-bottom: 60px;

    .title {
      text-transform: uppercase;
      font-size: 28px;
    }

  }

  .row-news {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 25px;

    .box-news {
      width: calc( (100% / 3) - 20px);

      .data-post {
        color: $gray;
        font-size: 14px;
        padding-top: 15px;
        padding-bottom: 10px;
      }

      .title-news {
        text-transform: uppercase;
        padding-bottom: 18px;
      }

      .description-news {
        color: $gray;
        font-size: 13px;
        padding-bottom: 15px;
      }

    }

  }

  .img {
    position: relative;
  }

  .stick-news {
    position: absolute;
    bottom: 5px;
    right: 0;
    display: flex;
    align-items: center;
    gap: 10px;
    background-color: rgba($color: black, $alpha: 0.8);
    color: $white;
    padding: 5px 12px;
    text-transform: uppercase;
    font-size: 12px;
    visibility: hidden;
  }

  .box-news:hover .stick-news {
    visibility: visible;
  }

}

</style>
