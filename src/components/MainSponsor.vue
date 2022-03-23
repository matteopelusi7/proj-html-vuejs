<template>
  <section>

    <div class="container">

      <div class="row box-title-sponsors">
        <h3 class="title-sponsors">Sponsors</h3>
        <p class="description-sponsors">Maecenas faucibus mollis interdum. Nullam id dolor id nibh ultricies vehicula ut id elit.</p>
      </div>

      <div class="row box-image-sponsors">
        <figure class="item-sponsors">
          <img src="../assets/img/banner-1.jpg" alt="">
        </figure>
        <figure class="item-sponsors">
          <img src="../assets/img/banner-2.jpg" alt="">
        </figure>
        <figure class="item-sponsors">
          <img src="../assets/img/banner-3.jpg" alt="">
        </figure>
        <figure class="item-sponsors">
          <img src="../assets/img/banner-4.jpg" alt="">
        </figure>
        <figure class="item-sponsors">
          <img src="../assets/img/banner-5.jpg" alt="">
        </figure>
        <figure class="item-sponsors">
          <img src="../assets/img/banner-6.jpg" alt="">
        </figure>
      </div>

    </div>

  </section>
</template>

<script>
export default {
  name: 'MainSponsor',
  
}
</script>

<style scoped lang="scss">

@import '../assets/scss/common.scss';

section {

  padding: 80px 0;
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
