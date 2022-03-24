<template>
  <section id="about">

    <div class="container">

      <div class="row">

        <div v-for="(el, i) in aboutList" :key="i" class="container-about">
          <div class="icon-wrapper">
            <i :class="el.icon"></i>
          </div>
          <div class="description-wrapper">
            <p class="title-about">{{ el.question }}</p>
            <p class="description-about">{{ el.description }}</p>
            <p class="more-info">{{ el.more }}</p>
          </div>
        </div>
        
      </div>

    </div>

  </section>
</template>

<script>
export default {
  name: 'MainAbout',
  data() {
    return {
      aboutList: [
        {
          question: 'Who we are',
          description: 'Donec id elit non mi porta gravida at eget me tus. Sed posuere consectetur estat lobo rtis. Cum sociis natoque.',
          more: 'Learn more',
          icon: 'fa-solid fa-trophy'
        },
        {
          question: 'What we do',
          description: 'Donec id elit non mi porta gravida at eget me tus. Sed posuere consectetur estat lobo rtis. Cum sociis natoque.',
          more: 'Learn more',
          icon: 'fa-solid fa-bolt'
        },
        {
          question: 'Why us?',
          description: 'Donec id elit non mi porta gravida at eget me tus. Sed posuere consectetur estat lobo rtis. Cum sociis natoque.',
          more: 'Learn more',
          icon: 'fa-solid fa-question'
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">

@import '../assets/scss/common.scss';

section {

  padding: 50px 10px;

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
      cursor: pointer;
    }

  }

}

</style>
