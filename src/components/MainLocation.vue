<template>
  <section id="location">

    <div class="container">
      <div class="row">

        <div class="title-wrapper">
          <h2 class="subtitle">Location</h2>
          <h1 class="title">Cb Building, grand conference room</h1>
        </div>

        <div class="description-location">
          <i class="fa-solid fa-paper-plane"></i>
          <p>11 GD Building, River Mall, New York, USA 8879</p>
        </div>

        <div>
          <p class="check">Check for Accomodations Here</p>
        </div>

        <div class="separator">
          <figure>
            <img src="../assets/img/1-item-2.jpg" alt="">
          </figure>
          <div class="date-wrapper">
            <i class="fa-solid fa-phone"></i>
            <p>+1-112-222--3344</p>
            <i class="fa-solid fa-envelope"></i>
            <p>Contact@TheKeynoteTheme.com</p>
          </div>
        </div>

      </div>
    </div>

  </section>
</template>

<script>
export default {
  name: 'MainLocation',
  
}
</script>

<style scoped lang="scss">

@import '../assets/scss/common.scss';

section {

  background-image: url('../assets/img/location-bg.jpg');
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
      font-size: 35px;
      font-weight: 700;
      padding-bottom: 50px;
    }

    .title {
      font-size: 30px;
      font-weight: 500;
    }

    .separator {
      text-align: center;
    }

    figure {
      padding-bottom: 10px;
    }

    .date-wrapper {
      display: flex;
      justify-content: center;
      gap: 20px;
      font-size: 16px;
    }

    .description-location {
      display: flex;
      gap: 10px;
      padding-bottom: 10px;
    }

    .check {
      color: $red;
      padding-bottom: 10px;
    }

  }

}

</style>
