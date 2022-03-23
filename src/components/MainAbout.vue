<template>
  <section>

    <div class="container">

      <div class="row">

        <div class="container-about">
          <div class="icon-wrapper">
            <i class="fa-solid fa-trophy"></i>
          </div>
          <div class="description-wrapper">
            <p class="title-about">Who we are</p>
            <p class="description-about">Donec id elit non mi porta gravida at eget me tus. Sed posuere consectetur estat lobo rtis. Cum sociis natoque.</p>
            <p class="more-info">Learn more</p>
          </div>
        </div>
        <div class="container-about">
          <div class="icon-wrapper">
            <i class="fa-solid fa-bolt"></i>
          </div>
          <div class="description-wrapper">
            <p class="title-about">What we do</p>
            <p class="description-about">Donec id elit non mi porta gravida at eget me tus. Sed posuere consectetur estat lobo rtis. Cum sociis natoque.</p>
            <p class="more-info">Learn more</p>
          </div>
        </div>
        <div class="container-about">
          <div class="icon-wrapper">
            <i class="fa-solid fa-question"></i>
          </div>
          <div class="description-wrapper">
            <p class="title-about">Why us?</p>
            <p class="description-about">Donec id elit non mi porta gravida at eget me tus. Sed posuere consectetur estat lobo rtis. Cum sociis natoque.</p>
            <p class="more-info">Learn more</p>
          </div>
        </div>

      </div>

    </div>

  </section>
</template>

<script>
export default {
  name: 'MainAbout',
  
}
</script>

<style scoped lang="scss">

@import '../assets/scss/common.scss';

section {

  padding: 50px 0;

  .row {
    display: flex;
    gap: 20px;
    justify-content: center;
  }

  .container-about {
    display: flex;
    justify-content: center;
    width: calc((100% / 3) - 25px );
    gap: 25px;
  }

  .icon-wrapper {
    color: $gray;
  }

  .description-wrapper {
    display: flex;
    flex-direction: column;
    gap: 15px;

    .title-about {
      text-transform: uppercase;
      font-weight: 600;
    }

    .description-about {
      color: $gray;
    }

    .more-info {
      color: $froly;
      font-style: italic;
    }

  }

}

</style>
