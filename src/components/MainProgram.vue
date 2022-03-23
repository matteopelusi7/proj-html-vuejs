<template>
  <section id="program">

    <div class="container">

      <div class="row title-row">

        <div class="title-box">
          <h4 class="title">Program</h4>
          <p class="description">This conference run through all 4 days from 23-26 May 2016. We also provide free lunch and coffee break in each day.</p>
        </div>

        <div class="more-info">
          <p>View Full Program</p>
        </div>

      </div>

      <div class="row row-description">

        <div class="box-wrapper">
          <div class="box-item">
            <p class="title-box">Day 1</p>
            <p>23 May 2016</p>
          </div>
          <div class="box-item">
            <p class="title-box">Day 2</p>
            <p>23 May 2030</p>
          </div>
          <div class="box-item">
            <p class="title-box">Day 3</p>
            <p>23 May 2030</p>
          </div>
          <div class="box-item">
            <p class="title-box">Day 4</p>
            <p>23 May 2030</p>
          </div>
          <div class="box-item">
            <p class="title-box">Day 5</p>
            <p>23 May 2030</p>
          </div>
          <div class="box-item">
            
          </div>
        </div>

        <div class="box-description">

          <div class="box-1">
            <div class="item-box-1">
              <i class="fa-solid fa-clock"></i>
              <p>09:00 - 10:30</p>
            </div>
            <div class="item-box-1">
              <i class="fa-solid fa-location-arrow"></i>
              <p>Room a</p>
            </div>
            <div class="item-box-1">
              <i class="fa-solid fa-user"></i>
              <p class="item-red">Laurence Francis</p>
            </div>
          </div>

          <div class="box-2">

            <div>
              <p class="title-box-2">Welcoming And Introduction</p>
            </div>
            <div>
              <p>Vestibulum id ligula porta felis euismond semper. Nullam quis risus edget urna mollis ornare vel eu leo. Donec ullamcorper nulla non meus auctor fringilla. Aenaen lacinia bibendum nulla sed consectetur...</p>
            </div>
            <div>
              <figure>
                <img src="../assets/img/speaker-8-150x150.jpg" alt="">
              </figure>
            </div>

          </div>

        </div>

      </div>

    </div>

  </section>
</template>

<script>
export default {
  name: 'MainProgram',
  
}
</script>

<style scoped lang="scss">

@import '../assets/scss/common.scss';

section {

  padding: 80px 10px;

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

  .box-wrapper {

    display: flex;
    justify-content: center;

    .box-item {
      width: calc( 100% / 6);
      background-color: $red;
      padding: 20px;
      color: $white;
      border-right: 2px solid #c72b11;

      &:first-child {
        background-color: #c72b11;
      }

      .title-box {
        font-weight: 700;
        padding-bottom: 7px;
        text-transform: uppercase;
      }

      p {
        font-size: 14px;
      }

    }

  }

  .box-description {
    width: 100%;
    background-color: #f7f7f7;
    color: $gray;
    display: flex;
    padding: 50px 80px;
    gap: 50px;

    .box-1 {

      width: 45%;

      .item-box-1 {
        display: flex;
        gap: 15px;
        padding: 10px 0;
        font-size: 13px;
      }

      p {
        text-transform: uppercase;
      }

      i {
        font-size: 16px;
      }

      .item-red {
        color: $red;
      }

    }

  }

  .box-2 {

    display: flex;
    flex-direction: column;
    gap: 20px;
    flex-grow: 1;

    .title-box-2 {
      font-size: 25px;
      font-weight: 500;
      text-transform: uppercase;
    }

    figure {
      width: 50px;
    }

  }

}

</style>
