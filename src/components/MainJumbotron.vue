<template>
  <section id="jumbo">

    <div class="container">
      <div class="row">

        <div class="title-wrapper">
          <h2 class="subtitle">Conference on</h2>
          <h1 class="title">Social Networks</h1>
        </div>

        <div class="separator">
          <figure>
            <img src="../assets/img/1-item-2.jpg" alt="">
          </figure>
          <div class="date-wrapper">
            <p class="date">23- 26 may 2019</p>
            <p class="date">San Francisco</p>
            <p class="date">8 Speakers</p>
          </div>
        </div>

        <div class="button-jumbo">
          <button class="button">Register online</button>
        </div>

      </div>
    </div>

  </section>
</template>

<script>
export default {
  name: 'MainJumbotron',
  
}
</script>

<style scoped lang="scss">

@import '../assets/scss/common.scss';

section {

  background-image: url('../assets/img/slider-1-bg.jpg');
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  color: $white;
  padding: 80px 10px;

  .row {
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    gap: 20px;

    .title-wrapper {
      text-transform: uppercase;
      text-align: center;
    }

    .subtitle {
      font-size: 45px;
      font-weight: 100;
      padding-bottom: 10px;
    }

    .title {
      font-size: 60px;
      font-weight: 700;
    }

    .separator {
      text-align: center;
    }

    figure {
      padding-bottom: 10px;
    }

    .date {

      &::after {
        content: ' /';
      }
    }

    .date-wrapper {
      display: flex;
      justify-content: center;
      gap: 20px;
      font-size: 16px;
      font-weight: 600;
      text-transform: uppercase;
    }

    .button {
      color: $white;
      background-color: #f62b0a;
      border: none;
      text-transform: uppercase;
      padding: 15px 25px;
      border-radius: 3px;
      font-weight: 600;
      cursor: pointer;
      margin-top: 5px;
    }

  }

}

</style>
